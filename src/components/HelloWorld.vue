<template>

<div class="all">
  

    
    
    
 <div class="sidebar">
            <div style="text-align:center;"><img src="coreui.png" alt="coreui" style="width: 100px;height: 70px;"></div>

            <div style="width: 170px;">
                
            </div>

            <div>
                THEME
                <br><br>
                <div style="display:flex;">
                    <div>
                        <i class="fa-solid fa-droplet"></i>
                    </div>
                    <div>
                         Colors
                    </div>
                </div>
                <br>
                <i class="fa-solid fa-pen"></i>
                 Typography
            </div>
        
            <div>
<br>
                COMPONENTS
            <br>
                <div class="base">
                    <div style="display :flex; justify-content: space-between;">
                        <div onclick="show()" style="margin: 8px;">
                            <span>
                                <i class="fa-solid fa-earth-americas"></i>
                            </span>
                            <span style="cursor:pointer;">
                                
                            </span>
                        </div>
                        <div style="margin: 8px;">></div>
                    </div>
                    <div class="sous_base" style="display: none;">
                        [sous-section]
                    </div>
                    
                </div>    
        
                
                <div class="button">
                    <div style="display :flex; justify-content: space-between;">
                        <div onclick="show2()" style="margin: 8px;" >
                            <i class="fa-solid fa-arrow-pointer"></i>
                           Buttons
                        </div>
                        <div style="margin: 8px;">></div> 
                    </div>  
                    <div class="sous_button" style="display: none;">
                        [sous-section]
                    </div>
                     
                </div>
                
                <div class="chart" style="display: flex;">
                    <div style="margin: 5px;">
                    <i class="fa-solid fa-clock"></i>
                    </div>
                    <div style="margin: 5px;">
                    Charts
                    </div>
                </div>
        
                <div class="forms">
                    <div style="display:flex; justify-content: space-between;">
                        <div onclick="show3()" style="margin: 8px;">
                            <i class="fa-solid fa-newspaper"></i>
                             Forms
                        </div>
                        <div style="margin: 8px;">></div>
                    </div>
                    <div class="sous_form" style="display: none;">
                    [sous-section]
                    </div>
                </div>
        
                <div class="icons">
                    <div style="display:flex; justify-content: space-between;">
                        <div onclick="show4()" style="margin: 8px;">
                            <i class="fa-solid fa-star"></i>
                             Icons
                        </div>
                        <div style="margin: 8px;">></div>
                         
                    </div>
                    <div class="sous_icon" style="display: none;">
                        [sous-section]
                    </div>
                   
                </div>   
                
                <div class="notification">
                    <div style="display :flex; justify-content: space-between;">
                        <div onclick="show5()" style="margin: 8px;">
                            <i class="fa-solid fa-bell"></i>
                             Notification
                        </div>
                        
                        <div style="margin: 8px;">></div>
                    </div>
                </div>
                    <div class="sous_notif" style="display: none;">
                        [sous-section]
                    </div>
               
                <div class="widget" style="display:flex;">
                    <div style="margin: 8px;">
                        <i class="fa-solid fa-newspaper"></i>
                    </div>
                    <div style="margin: 5px;">
                     Widget
                    </div>
                </div>
            </div>
            
<br>
            <div>
                EXTRAS
                <div class="pages" style="display : flex; justify-content: space-between;">

                    <div>
                        <div onclick="show6()" style="margin: 8px;">
                            <i class="fa-solid fa-star"></i>
                             Pages
                        </div>
                        
                    </div>

                    <div style="margin: 8px;">></div>
                </div>

                <div class="sous_page" style="display: none;">
                    [sous-section]
                </div>
            </div>
<br>
            <div>
                <div class="docs"><i class="fa-brands fa-dochub"></i> Docs</div>
                <div class="try">Try CoreUIPRO</div>
        
            </div>
                
            
        
        
        
            </div>

  





<div style="display:block;">
            <div class="navbar">
                
            
                <div class="nav_left">
                    <div class="tirait">
                    <div class="tirait1"></div>
                    <div class="tirait2"></div>
                    <div class="tirait3"></div>
                    </div>

                    <div>Dashboard</div>
                    <div>Users</div>
                    <div>Settings</div>
                </div>

                <div class="nav_right">
                    <i class="fa-solid fa-bell"></i>
                    <i class="fa-solid fa-list"></i>
                    <i class="fa-solid fa-envelope"></i>
                    

                </div>
            </div>
        
        
            <div class="section">
                <div style="margin-left: 40px;">Home /  Dashboard </div>
            </div>

            <div class="mainpart" id="app">
                <br>
                <div class="first" style="display: flex;">
                    <div class="users"></div>
                    <div class="income"></div>
                    <div class="rate"></div>
                    <div class="sessions"></div>
                </div>

                <br>

                <div class="sec">
                    <div class="traffic">
                        <div class="top"></div>
                          <div class="mid">
<div style="width: 600px;">
    <canvas id="myChart" width="400" height="200"></canvas>
    
    </div>
                            
                          </div>
                        <div class="bot"></div>
                    </div>
                </div>

 


                <!-- {{user}} {{income}} {{rate}} {{sessions}} -->
            </div>
  </div>




</div>   
 
  
</template>












<script>
import Chart from 'chart.js/auto';


// importation de la librairie charts.js permettant de créer des graph

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  mounted(){
    console.log('Component mounted.')

    const ctx = document.getElementById('myChart');

const labels = ['January', 'February', 'March', 'April', 'May', 'June', 'July'];
const data = {
  labels: labels,
  datasets: [{
    label: 'My First Dataset',
    data: [65, 59, 80, 81, 56, 55, 40],
    fill: false,
    borderColor: 'rgb(75, 192, 192)',
    tension: 0.1
  }]
};

    const myChart = new Chart(ctx, {
       type: 'line',
  data: data,
});

myChart;
  }
}
</script>


<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
