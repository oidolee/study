<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script src="https://unpkg.com/vue-router@3.0.1/dist/vue-router.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    
  
</head>
<body>
    <div id="app">
        <button v-on:click="getData">프레임워크목록</button>
    </div>
    <script>
        new Vue({
            el:'#app',
            methods : {
                getData : function(){
                    alert(12)
                    // axios.get('https://raw.githubusercontent.com/joshua1988/doit-vuejs/master/data/demo.json')
                    //     .then(function(response){
                    //         console.log(response)
                    //     });
                }
            }
        });
    </script>
</body>
      
</html>

-------------------------------이벤트 형식

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
  
</head>
<body>
    <div id="app">
        {{mesaage}}
        <wide-com v-on:show-log="printText"></wide-com>
    </div>
    <script>
        Vue.component('wide-com',{
            template : '<button v-on:click="showLog">show log</button>',
            methods : {
                showLog : function(){
                    this.$emit('show-log');
                }
            }
        });
        new Vue({
            el:'#app',
            data : {
               mesaage : 'hello!! haha' ,
            },
            methods : {
                printText : function(){
                    console.log("received an event")
                }
            }
        });
    </script>

</html>
