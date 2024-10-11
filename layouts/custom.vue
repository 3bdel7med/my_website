<template>
    <div id="viewport">
       <!-- Sidebar -->
       <div id="sidebar">
         <header>
           <NuxtLink to="/">Portofilo</NuxtLink>
         </header>
         <ul class="nav">
           <li class="mt-4">
             <NuxtLink to="/">
               <i class="fa-brands fa-phone"></i> Dashboard
             </NuxtLink>
           </li>
           <li class="mt-4" >
             <NuxtLink to="/">
               <i class="fa fa-home"></i> HOME
             </NuxtLink>
           </li>
           <br>
           <li class="mt-4 ml-5">
             <NuxtLink to="/dashboard/skill">
               <i class="fa fa-cogs"></i> SKILLS
             </NuxtLink>
           </li>
           <li class="mt-4">
             <NuxtLink to="/dashboard/cv">
               <i class="fas fa-briefcase"></i>CURRICULUM VITAE
             </NuxtLink>
           </li>
           <li class="mt-4">
             <NuxtLink to="/dashboard/about">
               <i class="fa fa-gear"></i> About
             </NuxtLink>
           </li>
           <li class="mt-4">
             <NuxtLink to="/dashboard/services">
               <i class="fa fa-wrench "></i> Services
             </NuxtLink>
           </li>
           <li class="mt-4">
             <NuxtLink to="/dashboard/contact">
               <i class="fa fa-phone"></i> Contact
             </NuxtLink>
           </li>
         </ul>
       </div>
       <!-- Content -->
       <div id="content">
         <nav class="navbar navbar-default">
           <div class="container-fluid">
             <ul class="nav navbar-nav navbar-right">
               <li class="mt-4">
                 <a href="#"><i class="zmdi zmdi-notifications text-danger"></i>
                 </a>
               </li>
             </ul>
           </div>
         </nav>
         <div class="container-fluid">
           
           <slot/>
         </div>
       </div>
     </div>
 </template>
 <style>
 @import url('https://fonts.googleapis.com/css?family=Roboto:300,400,400i,500');
 
 body {
   overflow-x: hidden;
   font-family: 'Roboto', sans-serif;
   font-size: 16px;
 }
 
 /* Toggle Styles */
 
 #viewport {
   padding-left: 250px;
   -webkit-transition: all 0.5s ease;
   -moz-transition: all 0.5s ease;
   -o-transition: all 0.5s ease;
   transition: all 0.5s ease;
 }
 
 #content {
   width: 100%;
   position: relative;
   margin-right: 0;
 }
 
 /* Sidebar Styles */
 
 #sidebar {
   z-index: 1000;
   position: fixed;
   left: 250px;
   width: 250px;
   height: 100%;
   margin-left: -250px;
   overflow-y: auto;
   background: #37474F;
   -webkit-transition: all 0.5s ease;
   -moz-transition: all 0.5s ease;
   -o-transition: all 0.5s ease;
   transition: all 0.5s ease;
 }
 
 #sidebar header {
   background-color: #263238;
   font-size: 20px;
   line-height: 52px;
   text-align: center;
 }
 
 #sidebar header a {
   color: #fff;
   display: block;
   text-decoration: none;
 }
 
 #sidebar header a:hover {
   color: #fff;
 }
 
 #sidebar .nav{
   
 }
 
 #sidebar .nav a{
   background: none;
   border-bottom: 1px solid #455A64;
   color: #CFD8DC;
   font-size: 14px;
   padding: 16px 24px;
 }
 
 #sidebar .nav a:hover{
   background: none;
   color: #ECEFF1;
 }
 
 #sidebar .nav a i{
   margin-right: 16px;
 }
 </style>
 