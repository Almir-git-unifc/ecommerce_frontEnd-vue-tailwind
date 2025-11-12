<template>
<div id="contact" class=" bg-pink-950 px-4 py-12 sm:px-6 lg:px-8" >

  <div class="mx-auto max-w-7xl">
    <div class="mb-12 text-center">
      <h1 class="mb-4 font-serif text-4xl font-bold text-white">Contact Us</h1>

      <p class="mx-auto max-w-2xl text-lg text-gray-200">Have questions about our jewelry? Our jewelry experts are here to help you.</p>
    </div>

    <div class="grid grid-cols-1 gap-12 lg:grid-cols-2">
      <div class="rounded-lg border border-gray-100 bg-white p-8 shadow-xl">
        <h2 class="mb-6 font-serif text-2xl font-semibold text-gray-900">Sned Us a Message</h2>

        <form class="space-y-6">
          <div>
            <label for="name" class="mb-1 block text-sm font-medium text-gray-800"> Your Name </label>

            <input type="text" id="name" class="w-full rounded-lg border border-gray-200 px-4 py-3 focus:border-transparent focus:ring-2 focus:ring-pink-500" placeholder="Your name" />
          </div>

          <div>
            <label for="email" class="mb-1 block text-sm font-medium text-gray-800"> Email Address </label>
            <input type="text" id="email" class="w-full rounded-lg border border-gray-200 px-4 py-3 focus:border-transparent focus:ring-2 focus:ring-pink-500" placeholder="Your@email.com" />
          </div>

          <!--  Aos 53:10 min. -->
          <div>
            <label for="message" class="mb-1 block text-sm font-medium text-gray-800"> 
              Your Message 
            </label>
            <textarea rows="5" id="message" class="w-full rounded-lg border border-gray-200 px-4 py-3 focus:border-transparent focus:ring-2 focus:ring-pink-500" placeholder="Tell us about your fragrance needs..."
            >              
            </textarea>
          </div>

          <button class="w-full rounded-lg bg-pink-700 px-6 py-3 font-medium text-white shadow-md transition duration-300 hover:bg-pink-800"
          >
                Send Message
          </button>
        </form>
      </div>


      <!--  Quadrado lado direito -->
      <div class="space-y-8">
        <div class="bg-white p-8 rounded-1h shadow-x1 border border-gray-100"> 
          <h2 class="text-2xl font-serif font-semibold text-gray-900 mb-6">
            Contact Informations
          </h2>
          <div class="space-y-6">
            <div class="flex items-start">      
              <div class="bg-pink-200 p-3 rounded-full mr-4"
              >
                 <!-- Icone  -->
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 48 48">
                <path fill="#731154" d="M46.483 14.556C45.925 32.293 31.372 46.5 13.5 46.5c-6.833 0-12-5.335-12-12.069a4.5 4.5 0 0 1 2.829-4.178l6.165-2.466a5.5 5.5 0 0 1 5.932 1.217l3.076 3.077c.136.136.289.152.382.124a18.55 18.55 0 0 0 12.32-12.32c.029-.094.013-.247-.123-.383l-3.077-3.076a5.5 5.5 0 0 1-1.217-5.932l2.466-6.165A4.5 4.5 0 0 1 34.431 1.5c7.365 0 12.166 5.861 12.052 13.056" />
              </svg>
              </div>

              <div>
                 <h3 class="text-lg font-medium text-gray-900"
                >
                   Phone
                </h3>
                <p class="text-gray-800">+1 (234) 567-8900</p>
                <p class="text-gray-600 mb-6">Mon-Fri: 9am-6pm</p> </div>
              </div>
            </div>

            <div class="flex items-start">      
              <div class="bg-pink-200 p-3 rounded-full mr-4 "
              >
              <span></span>
                 <!-- <Icon icon="fa-solid:envelope" class="text-pink-950 text-lg"/> Icone anterior -->
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                  <g fill="none">
                    <path fill="#731154" d="M1 3.5h22v17H1z" />
                    <path fill="#cf8fd9" fill-rule="evenodd" d="M1 7.721v-1.79l11 7.174L23 5.93v1.79l-10.59 6.907l-.41.267l-.41-.267z" clip-rule="evenodd" />
                  </g>
                </svg>
              </div>

              <div>
                 <h3 class="text-lg font-medium text-gray-900"
                >
                   Email
                </h3>
                <p class="text-gray-800">contact@jewelrylux.com</p>
                <p class="text-gray-600 mb-6">support@jewelrylux.com</p> 
              </div>

            </div>

            <div class="flex items-start">      
              <div class="bg-pink-200 p-3 rounded-full mr-4"
              >
                 <!-- <Icon icon="map-marker" class="text-pink-950 text-lg"/> Icone anterior -->
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 18 24">
                  <path fill="#731154" d="M8.075 23.52C1.264 13.642 0 12.629 0 9c0-4.971 4.029-9 9-9s9 4.029 9 9c0 3.629-1.264 4.64-8.075 14.516a1.126 1.126 0 0 1-1.847.004l-.002-.004zM9 12.75a3.75 3.75 0 1 0 0-7.5a3.75 3.75 0 0 0 0 7.5" />
                </svg>
              </div>

              <div>
                 <h3 class="text-lg font-medium text-gray-900"
                >
                   Our jewelry store
                </h3>
                <p class="text-gray-800">123 jewelry Street</p>
                <p class="text-gray-600">Amsterdam - Netherlands 75001</p>                 
              </div>
              </div>

              <div class="mt-24">
                  <h3 class="text-xl font-semibold text-gray-900 mb-4">
                       Follow Us
                  </h3> 
                  <div class="flex space-x-4">
                      <a href="#" class="bg-pink-200 hover:bg-gray-200 p-3 rounded-full transition duration-300">
                               <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                                    <path fill="#731154" d="M7.8 2h8.4C19.4 2 22 4.6 22 7.8v8.4a5.8 5.8 0 0 1-5.8 5.8H7.8C4.6 22 2 19.4 2 16.2V7.8A5.8 5.8 0 0 1 7.8 2m-.2 2A3.6 3.6 0 0 0 4 7.6v8.8C4 18.39 5.61 20 7.6 20h8.8a3.6 3.6 0 0 0 3.6-3.6V7.6C20 5.61 18.39 4 16.4 4zm9.65 1.5a1.25 1.25 0 0 1 1.25 1.25A1.25 1.25 0 0 1 17.25 8A1.25 1.25 0 0 1 16 6.75a1.25 1.25 0 0 1 1.25-1.25M12 7a5 5 0 0 1 5 5a5 5 0 0 1-5 5a5 5 0 0 1-5-5a5 5 0 0 1 5-5m0 2a3 3 0 0 0-3 3a3 3 0 0 0 3 3a3 3 0 0 0 3-3a3 3 0 0 0-3-3" />
                              </svg>
                      </a>
              
                      <a href="#" class="bg-pink-200 hover:bg-gray-200 p-3 rounded-full transition duration-300">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                                <path fill="#731154" d="M15.12 5.32H17V2.14A26 26 0 0 0 14.26 2c-2.72 0-4.58 1.66-4.58 4.7v2.62H6.61v3.56h3.07V22h3.68v-9.12h3.06l.46-3.56h-3.52V7.05c0-1.05.28-1.73 1.76-1.73" />
                            </svg>                            
                      </a>

                      <!-- Aos 56:41 min. -->              
                      <a href="#" class="bg-pink-200 hover:bg-gray-200 p-3 rounded-full transition duration-300">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                                  <path fill="#731154" d="M22.46 6c-.77.35-1.6.58-2.46.69c.88-.53 1.56-1.37 1.88-2.38c-.83.5-1.75.85-2.72 1.05C18.37 4.5 17.26 4 16 4c-2.35 0-4.27 1.92-4.27 4.29c0 .34.04.67.11.98C8.28 9.09 5.11 7.38 3 4.79c-.37.63-.58 1.37-.58 2.15c0 1.49.75 2.81 1.91 3.56c-.71 0-1.37-.2-1.95-.5v.03c0 2.08 1.48 3.82 3.44 4.21a4.2 4.2 0 0 1-1.93.07a4.28 4.28 0 0 0 4 2.98a8.52 8.52 0 0 1-5.33 1.84q-.51 0-1.02-.06C3.44 20.29 5.7 21 8.12 21C16 21 20.33 14.46 20.33 8.79c0-.19 0-.37-.01-.56c.84-.6 1.56-1.36 2.14-2.23" />
                            </svg>
                      </a>
                  </div>
              </div>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>
