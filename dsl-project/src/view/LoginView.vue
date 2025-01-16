<script setup>

  
  const handleGoogleLogin = async () => {
    try {
      // You would normally use Google API to authenticate users.
      console.log('Google login button clicked!')
      // Placeholder: Add your Google login logic here, for example using Google API or firebase.auth.
    } catch (error) {
      console.error('Google login error:', error)
    }
  }
  </script>

<template>
    <div 
      class="min-h-screen bg-gray-100 flex items-center justify-center p-4" 
      style="background-image: url('/src/assets/img/background.jpg'); background-size: cover; background-position: center;">
      <div class="max-w-md w-full bg-white rounded-lg shadow-lg p-8">
        <!-- Logo Section -->
        <div class="text-center mb-8">
          <img 
            src="/src/assets/img/logo.jpg" 
            alt="Logo" 
            class="mx-auto h-16 w-16 mb-4"
          />
          <h2 class="text-2xl font-bold text-gray-900">MFU DSL EQUEUE</h2>
          <p class="text-sm text-gray-600">ระบบจองคิว กยศ มหาวิทยาลัยแม่ฟ้าหลวง</p>
        </div>
    
        <!-- Google Login Button -->
        <div class="space-y-6">
          <button
            @click="handleGoogleLogin"
            class="w-full flex items-center justify-center py-3 px-6 border border-transparent rounded-lg shadow-lg text-sm font-medium text-white bg-gradient-to-r from-blue-500 to-blue-600 hover:from-blue-600 hover:to-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition-all duration-300 transform hover:scale-105"
          >
            <i class="fab fa-google mr-3 text-lg"></i>
            <span>ลงชื่อเข้าใช้งานระบบ</span>
          </button>
        </div>
      </div>
    </div>
  </template>

  
  