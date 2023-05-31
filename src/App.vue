<script setup>
// Burger menus
document.addEventListener('DOMContentLoaded', function() {
    // open
    const burger = document.querySelectorAll('.navbar-burger');
    const menu = document.querySelectorAll('.navbar-menu');

    if (burger.length && menu.length) {
        for (var i = 0; i < burger.length; i++) {
            burger[i].addEventListener('click', function() {
                for (var j = 0; j < menu.length; j++) {
                    menu[j].classList.toggle('hidden');
                }
            });
        }
    }

    // close
    const close = document.querySelectorAll('.navbar-close');
    const backdrop = document.querySelectorAll('.navbar-backdrop');

    if (close.length) {
        for (var i = 0; i < close.length; i++) {
            close[i].addEventListener('click', function() {
                for (var j = 0; j < menu.length; j++) {
                    menu[j].classList.toggle('hidden');
                }
            });
        }
    }

    if (backdrop.length) {
        for (var i = 0; i < backdrop.length; i++) {
            backdrop[i].addEventListener('click', function() {
                for (var j = 0; j < menu.length; j++) {
                    menu[j].classList.toggle('hidden');
                }
            });
        }
    }
});

</script>

<template>
<section class="pt-6 pb-20 bg-gray-50 overflow-hidden">
  <div class="container mx-auto px-4">
    <div class="mb-6">
      <div class="flex items-center justify-between px-6 py-3.5 bg-white border border-gray-100 rounded-full">
        <div class="w-auto">
          <div class="flex flex-wrap items-center">
            <div class="w-auto"><a href="#"></a></div>
          </div>
        </div>
        <div class="w-auto">
          <div class="flex flex-wrap items-center">
            <div class="w-auto hidden lg:block">
              <ul class="flex items-center justify-center">
                <li class="mr-9"><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">How It Works</a></li>
                <li class="mr-9"><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">Pricing</a></li>
                <li class="mr-9"><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">FAQ</a></li>
                <li><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">Testimonials</a></li>
              </ul>
            </div>
          </div>
        </div>
        <div class="w-auto">
          <div class="flex flex-wrap items-center">
            <div class="w-auto hidden lg:block">
              <div class="flex flex-wrap -m-2">
                <div class="w-full md:w-auto p-2"><a class="block w-full px-4 py-2.5 text-sm text-center text-gray-900 font-bold bg-white hover:bg-gray-50 focus:ring-4 focus:ring-gray-200 border rounded-full" href="#">Log In</a></div>
                <div class="w-full md:w-auto p-2"><a class="block w-full px-4 py-2.5 text-sm text-center text-white font-bold bg-blue-500 hover:bg-blue-600 focus:ring-4 focus:ring-blue-200 rounded-full" href="#">Ask Me Anything</a></div>
              </div>
            </div>
            <div class="w-auto lg:hidden"><a class="inline-block" href="#">
              <svg class="navbar-burger text-blue-500" width="45" height="45" viewBox="0 0 56 56" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect width="56" height="56" rx="28" fill="currentColor"></rect>
                <path d="M37 32H19M37 24H19" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
              </svg></a></div>
          </div>
        </div>
      </div>
      <div class="navbar-menu fixed top-0 left-0 bottom-0 w-4/6 sm:max-w-xs z-50 hidden">
        <div class="navbar-backdrop fixed inset-0 bg-gray-800 opacity-80"></div>
        <nav class="relative z-10 px-9 pt-8 bg-white h-full overflow-y-auto">
          <div class="flex flex-wrap justify-between h-full">
            <div class="w-full">
              <div class="flex items-center justify-between -m-2">
                <div class="w-auto p-2"><a class="inline-block" href="#"><img src="" alt=""></a></div> // zanrly-assets/logos/zanrly-logo.sv
                <div class="w-auto p-2"><a class="inline-block navbar-burger" href="#">
                  <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M6 18L18 6M6 6L18 18" stroke="#111827" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
                  </svg></a></div>
              </div>
            </div>
            <div class="flex flex-col justify-center py-8 w-full">
              <ul>
                <li class="mb-9"><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">Features</a></li>
                <li class="mb-9"><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">Solutions</a></li>
                <li class="mb-9"><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">Resources</a></li>
                <li><a class="inline-block text-sm font-bold text-gray-900 hover:text-gray-700" href="#">Pricing</a></li>
              </ul>
            </div>
            <div class="flex flex-col justify-end w-full pb-8">
              <div class="flex flex-wrap -m-2">
                <div class="w-full p-2"><a class="block w-full px-4 py-2.5 text-sm text-center text-gray-900 font-bold bg-white hover:bg-gray-50 focus:ring-4 focus:ring-gray-200 border rounded-full" href="#">Log In</a></div>
                <div class="w-full p-2"><a class="block w-full px-4 py-2.5 text-sm text-center text-white font-bold bg-blue-500 hover:bg-blue-600 focus:ring-4 focus:ring-blue-200 rounded-full" href="#">Get Started</a></div>
              </div>
            </div>
          </div>
        </nav>
      </div>
    </div>
    <div class="flex flex-wrap justify-center -m-4">
      <div class="w-full md:w-auto p-4"><img class="mx-auto" src="https://res.cloudinary.com/dylevfpbl/image/upload/v1685547162/landingpage/image_1.png" alt=""></div>
      <div class="w-full md:flex-1 p-4">
        <div class="flex flex-col justify-center items-center p-8 h-full text-center bg-white rounded-3xl">
          <div class="max-w-lg">

            <h1 class="font-heading mb-6 text-5xl text-gray-900 font-black tracking-tight">
              <span>Ask a Privacy Expert&nbsp;</span><span class="text-blue-500">anything</span>
            </h1>
            <p class="mb-8 text-xl font-bold">I have spent years studying and building in the crypto and privacy space. Save time researching and get all of your questions answered with me.</p>
            <div class="flex flex-wrap justify-center -m-2">
              <div class="w-full md:w-auto p-2"><a class="block w-full px-4 py-2.5 text-sm text-center text-white font-bold bg-blue-500 hover:bg-blue-600 focus:ring-4 focus:ring-blue-200 rounded-full" href="#">Get Started</a></div>
              <div class="w-full md:w-auto p-2"><a class="block w-full px-4 py-2.5 text-sm text-center text-gray-900 font-bold bg-gray-50 hover:bg-gray-200 focus:ring-4 focus:ring-gray-200 rounded-full" href="#">Watch Video</a></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
                
      <section class="py-10 bg-gray-50 overflow-hidden">
        <div class="container mx-auto px-4">
          <div class="py-16 px-8 bg-white rounded-3xl">
            <div class="max-w-7xl mx-auto">
              <h2 class="font-heading max-w-xl mb-20 text-4xl md:text-5xl text-gray-900 font-black tracking-tight">How It Works</h2>
              <div class="flex flex-wrap -m-3">
                <div class="w-full md:w-1/2 lg:w-1/4 p-3">
                  <div class="flex flex-wrap items-center -m-3 mb-2">
                    <div class="w-auto p-3">
                      <div class="flex items-center justify-center w-16 h-16 text-xl text-gray-900 font-black bg-gray-100 rounded-full">1</div>
                    </div>
                    <div class="flex-1 p-3">
                      <div class="bg-gray-200 h-px"></div>
                    </div>
                  </div>
                  <div class="md:w-3/4">
                    <h3 class="font-heading mb-4 text-2xl text-gray-900 font-bold">Deposit</h3>
                    <p class="text-gray-700 font-bold">You submit a question on any topic  and deposit 5 USD of XMR.</p>
                  </div>
                </div>
                <div class="w-full md:w-1/2 lg:w-1/4 p-3">
                  <div class="flex flex-wrap items-center -m-3 mb-2">
                    <div class="w-auto p-3">
                      <div class="flex items-center justify-center w-16 h-16 text-xl text-white font-black bg-blue-500 rounded-full">2</div>
                    </div>
                    <div class="flex-1 p-3">
                      <div class="bg-gray-200 h-px"></div>
                    </div>
                  </div>
                  <div class="md:w-3/4">
                    <h3 class="font-heading mb-4 text-2xl text-gray-900 font-bold">We Chat</h3>
                    <p class="text-gray-700 font-bold">We chat about your question until you are satisfied.</p>
                  </div>
                </div>
                <div class="w-full md:w-1/2 lg:w-1/4 p-3">
                  <div class="flex flex-wrap items-center -m-3 mb-2">
                    <div class="w-auto p-3">
                      <div class="flex items-center justify-center w-16 h-16 text-xl text-gray-900 font-black bg-gray-100 rounded-full">3</div>
                    </div>
                    <div class="flex-1 p-3">
                      <div class="bg-gray-200 h-px"></div>
                    </div>
                  </div>
                  <div class="md:w-3/4">
                    <h3 class="font-heading mb-4 text-2xl text-gray-900 font-bold">Return Deposit</h3>
                    <p class="text-gray-700 font-bold">After we chat, I return your 5 USD XMR deposit back to you.</p>
                  </div>
                </div>
                <div class="w-full md:w-1/2 lg:w-1/4 p-3">
                  <div class="flex flex-wrap items-center -m-3 mb-2">
                    <div class="w-auto p-3">
                      <div class="flex items-center justify-center w-16 h-16 text-xl text-gray-900 font-black bg-gray-100 rounded-full">4</div>
                    </div>
                    <div class="flex-1 lg:hidden p-3">
                      <div class="bg-gray-200 h-px"></div>
                    </div>
                  </div>
                  <div class="md:w-3/4">
                    <h3 class="font-heading mb-4 text-2xl text-gray-900 font-bold">You Tip?</h3>
                    <p class="text-gray-700 font-bold">You tip me for whatever value you believe I provided.</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
                
      <section class="py-10 bg-gray-50 overflow-hidden">
        <div class="container mx-auto px-4">
          <div class="py-10 px-8 bg-white rounded-3xl">
            <div class="max-w-7xl mx-auto">
              <div class="flex flex-wrap -m-8">
                <div class="w-full md:w-1/2 p-8">
                  <div class="py-9 md:max-w-md">
      <span class="inline-block mb-5 text-sm text-blue-500 font-bold uppercase tracking-widest">Pricing</span>
                    <h2 class="font-heading mb-4 text-4xl text-gray-900 font-black tracking-tight">Simple Pricing</h2>
                    <p class="mb-8 text-gray-700 font-bold">You pay me for whatever value you think I provided you. You are required to place a 5 USD XMR deposit to ask a question. This deposit will be returned to you. </p>
                    <div class="flex flex-wrap -m-2">
                      
                      <div class="w-auto p-2">
                        
                      </div>
                      
                      <div class="w-auto p-2">
                        
                      </div>
                    </div>
                  </div>
                </div>
                <div class="w-full md:w-1/2 p-8">
                  <div class="py-24 px-8 text-center h-full bg-gray-100 rounded-3xl">
                    <div class="flex flex-col justify-between h-full">
                      <div class="flex-initial mb-10">
      <span class="inline-block mb-3.5 text-gray-900 font-black uppercase">ASK A Question</span>
                        <h2 class="font-heading mb-4 text-5xl md:text-7xl text-blue-500 font-black tracking-tight">
      <span>$5</span><span class="text-xl">USD</span>
      </h2>
                        <p class="text-gray-400 font-bold">A Deposit that will be refunded to you after we chat.</p>
                      </div>
                      <div class="flex-initial">
                        <div class="flex flex-wrap justify-center -m-2">
                          <div class="w-full p-2"><a class="block md:max-w-xs mx-auto w-full px-8 py-3.5 text-lg text-center text-white font-bold bg-blue-500 hover:bg-blue-600 focus:ring-4 focus:ring-blue-200 rounded-full" href="#">Ask Me Now</a></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
                
      <section class="py-10 bg-gray-50 overflow-hidden">
        <div class="container mx-auto px-4">
          <div class="py-16 px-8 bg-white border border-gray-100 rounded-3xl">
            <div class="max-w-7xl mx-auto">
              <div class="flex flex-wrap lg:items-center -m-8">
                <div class="w-full md:w-1/2 p-8"><img class="mx-auto md:ml-0 rounded-3xl" src="https://res.cloudinary.com/dylevfpbl/image/upload/v1685547106/landingpage/image_2_-min.png" alt=""></div>
                <div class="w-full md:w-1/2 p-8">
                  <p class="mb-10 text-2xl font-bold">"Had some questions about accepting XMR for my business idea and Dgoon helped me out a ton with btcpayserver and my business idea. Well worth it!"</p>
                  <h3 class="font-heading text-2xl text-gray-900 font-black">Anon Asker</h3>
                  
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

</template>

<style scoped>
</style>
