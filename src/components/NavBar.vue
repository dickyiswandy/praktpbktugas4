<template>
    <nav class="navbar">
      <div class="container">
        <a class="navbar-brand" href="#">LaundryCalculator</a>
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="#home">Beranda</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#services">Layanan</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#about">Tentang</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact">Kontak</a>
          </li>
        </ul>
      </div>
    </nav>
  </template>
  
  <style scoped>
  .navbar {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: #333;
    overflow: hidden;
    font-family: Arial, sans-serif;
    display: flex; 
    justify-content: space-between; 
    z-index: 999; /* agar navbar tampil di atas konten */
  }
  
  .navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%; 
  }
  
  .navbar a {
    color: #f2f2f2;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
  }
  
  .navbar a:hover {
    background-color: #ddd;
    color: black;
  }
  
  .navbar .navbar-brand {
    font-size: 1.8em;
    font-weight: bold;
    margin-right: auto; 
  }
  
  .navbar .navbar-nav {
    list-style: none; 
    display: flex; 
    margin: 0; 
    padding: 0; 
  }
  
  .navbar .navbar-nav .nav-item {
    padding: 0 10px; 
  }
  
  .navbar .navbar-nav .nav-link {
    color: #f2f2f2;
    text-decoration: none;
  }
  </style>
  