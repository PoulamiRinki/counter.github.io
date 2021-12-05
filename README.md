<!DOCTYPE html>
< html>
<html lang="en">
    <head> 
        <meta charset="UTF-8"> 
        <meta http-equiv="X-UA-Compatible" content="IE=edge"> 
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>Document</title> 
         <link rel="stylesheet" href="index.css" />
        </head>
        <body> 
            <div class="main-project-wrapper">
                 <div class="project-6-page-wrapper">
                      <h2> Counter</h2> 
                      <div class="project-6-wrapper"> 
                          <div class="counter-box-wrapper"> 
                              <div class="counter-number" id="counter-placeholder"> 0 </div> 
                              <button class="count-btns" id="btn-increment"> Increment </button> 
                              <button class="count-btns" id="btn-decrement"> Decrement </button> 
                            </div> 
                        </div> 
                    </div> 
                </div> 
                <script>
                  .project-6-page-wrapper{
     background-color: rgb(56, 23, 4);
      display: flex; 
      justify-content: center;
       align-content: center; 
       flex-direction: column; 
       align-items: center; 
    } 
    .project-6-page-wrapper >h2{ 
        padding: 10px 35px;
         margin-bottom: 10px;
          border: 1px solid rgb(233, 201, 174);
           text-align: center; 
           color: rgb(192, 231, 243); 
           font-family: Arial, Helvetica, sans-serif; 
        }
         .project-6-wrapper{
              width: 100%; 
              height: 400px;
              background-color: rgb(202, 114, 73); 
            }
             .counter-box-wrapper{
                  width: auto;
                   margin: 50px; 
                   height: 300px;
                    background-color: rgb(192, 166, 137);
                     box-shadow: 0px 0px 10px 10px rgb(71, 52, 22); 
                     text-align: center;
                     }
                      .counter-number{ 
                          font-size: 150px;
                           color: white;
                        } 
                        .count-btns{ 
                            padding: 10px;
                             width: auto;
                              background-color: rgb(85, 53, 2);
                               font-size: 18px;
                                cursor: pointer;
                                 margin-top: 10px;
                                  margin-right: 5px; 
                                  font-family: Arial, Helvetica, sans-serif; 
                                  border-radius: 10px;
                                   border: 2px solid rgb(1, 250, 237);
                                    color: white; 
                                    outline: none;
                                 }
                                  .count-btns:hover{ 
                                      background-color: rgb(133, 70, 42); 
                                    }
                  var counterPlaceHolder = document.getElementById("counter-placeholder");
var btnIncrement = document.getElementById("btn-increment");
var btnDecrement = document.getElementById("btn-decrement");
var number = 0;
function changeColor(number){ 
    var color = "";
     if(number < 0 ){
          color = "red"; 
        }
        else if (number > 0 ){
             color = "green"; 
            }
            else{ 
                color="white";
             } 
                return color;
            }
btnIncrement.addEventListener("click", function(){ 
    number++; 
    counterPlaceHolder.innerHTML = number; 
    counterPlaceHolder.style.color = changeColor(number);
});

btnDecrement.addEventListener("click", function(){ 
    number--; 
    counterPlaceHolder.innerHTML = number; 
    counterPlaceHolder.style.color = changeColor(number);
  });                
 </script>
 </body>
 </html>
