<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script src="https://unpkg.com/vue-router@3.0.1/dist/vue-router.js"></script>
</head>

<body>
    <div id="app">
        <p>{{ reversedMesaage }}</p>
    </div>
    <script>
        new Vue({
            el:'#app',
            data : {
                message : 'Hello vue.js!!'
            },
            computed : {
                reversedMesaage : function(){
                    return this.message.split('').reverse().join('');
                }
            }
        });
    </script>
  

</body>

</html>
