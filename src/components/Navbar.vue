<template>
    <div class="q-pa-none">
      
        <q-header elevated class="bg-dark text-white">
          <q-toolbar>
         
          
            <div class="column">
          <q-toolbar-title class=" big-text" >Toko Kulim</q-toolbar-title>
            <q-tabs no-caps  indicator-color="transparent" class="text-white" v-model="tab">
                <q-tab name="home" label="Home" />
                <q-tab name="produk" label="Produk" />
                <q-tab name="kategori" label="Kategori" />
            </q-tabs>
            </div>

            <q-space />
            <q-input dark borderless v-model="text" input-class="text-right" class="q-ml-md">
          <template v-slot:append>
            <q-btn round color="dark" icon="search" />
          </template>
          </q-input>
            <q-btn round color="dark" icon="shopping_cart" />
            <q-btn round color="dark" icon="account_circle" />
          </q-toolbar>
        </q-header>
  
      
    </div>
  </template>
  

  