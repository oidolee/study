<?php

use Illuminate\Support\Facades\Route;
use Illuminate\Support\Facades\Auth;


/*
|--------------------------------------------------------------------------
| Web Routes
|--------------------------------------------------------------------------
|
| Here is where you can register web routes for your application. These
| routes are loaded by the RouteServiceProvider within a group which
| contains the "web" middleware group. Now create something great!
|
*/

use App\Http\Controllers\HomeController;
use App\Http\Controllers\ProjectController;
use App\Http\Controllers\TaskContoller;

Route::get('/', [HomeController::class, 'index']);

// Route::get('/hello', function () {
//     return view('hello');
// });

Route::get('/hello', [HomeController::class, 'hello']);


// Route::get('contact', function(){
//     return view('contact');
// });

Route::get('/contact', [HomeController::class, 'contact']);

Route::get('/projects', [ProjectController::class, 'index']);

Route::prefix('/tasks')->middleware('auth')->group(function(){
    Route::get('/', [TaskContoller::class, 'index']);

    Route::get('/create', [TaskContoller::class, 'create']);
    
    Route::post('/', [TaskContoller::class, 'store']);
    
    Route::get('/{task}', [TaskContoller::class, 'show']);
    
    Route::get('/{task}/edit', [TaskContoller::class, 'edit']);
    
    Route::put('/{task}', [TaskContoller::class, 'update']);
    
    Route::delete('/{task}', [TaskContoller::class, 'destroy']);
});


Auth::routes();

Route::get('/home', [App\Http\Controllers\HomeController::class, 'index'])->name('home');

