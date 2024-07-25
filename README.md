# Task-2<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http.equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewpoint" content="width=device-width, initial-scale=1.0">
        <title>ToDo List</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <header>
            <nav class="container">
                <div class="logo">
                    <img src="ToDo.png" alt="ToDo List">
                    <p>ToDo List</p>
                </div>
                <ul>
                    <a href="ToDo.html">
                        <li>Home</li>
                    </a>
                    <a href="main">
                        <li>Contacts</li>
                    </a>
                    <a href="main">
                        <li>Sign in</li>
                    </a>    
                </ul>
            </nav>
        </header>
        <div class="main">
            <img src="scroll.png" alt="scroll image">
            <div class="content">
                <div class="container">
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                    <div class="todo">
                        <input class="todo_value" type="text" placeholder="(empty)">
                        <input class="todo_checkbox" type="checkbox">
                    </div>
                </div>
            </div>
        </div>
    </body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    background-image: url();
    background-size: cover;
    background-position: center;
}
header{
    width: 100%;
    position: sticky;
    top:0;
    z-index: 1;
    background: transparent;
}
header .container{
    height: 10vh;
    width: 100%;
    margin: 0 auto;
    padding:0 50px;
}
.logo{
    display: flex;
    gap: 14px;
    align-items: center;
}
.logo img{
    height: 35px;
    width: 30px;
}
.logo p{
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 20px;
    font-weight: 550;
    cursor: default;
}
a{
    text-decoration: none;
    color: white;
}
ul{
    display:flex;
    gap: 14px;
    list-style: none;
}
li{
    font-size: 20px;
}
nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 14px;
}
.main{
    width:100%;
    height: 90vh;
    position: absolute;
}
.main img{
    display: block;
    margin:auto;
    height: 100%;
    filter: drop-shadow(20px 20px 40px rgb(0, 0, 0))
}
.content{
    width: 100%;
    height: 100%;
    display: block;
    margin: auto;
    position: absolute;
    top: 0;
    left: 0;
}
.content .container{
    justify-content: center;
    display: flex;
    flex-direction: column;
    width: 300px;
    margin: auto;
    height: 100%;
}
.todo{
    cursor: url("Quill.png")6 19,auto;
    display: flex;
    padding: 14px;
}
.todo_value{
    cursor: inherit;
    background: transparent;
    border: none;
    outline: none;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 15px;
    font-weight: bold;
    flex-grow: 1;
    border-bottom: 2px solid rgb(94, 41, 21);
}    
.todo_checkbox{
    cursor: inherit;
}
.todo:has(.todo_checkbox:checked){
    color: rgb(84, 35, 0);
    background: rgba(0, 0, 0, 0.13);
    text-decoration: line-through 1.5px;
    order: 1;
}
