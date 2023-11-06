# flask_5_tailwind


## This is the hw 
<img width="1017" alt="Screen Shot 2023-11-05 at 9 06 32 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/647f145f-6981-4443-8999-18e6a6e721df">
website: https://flaskhw-404222.ue.r.appspot.com/


## Step 1
I went online and I downloaded a cat video.

## Step 2 - Google Cloud CDN
I created a bucket using Google Cloud and changed the access to public. From here, I was able to get a url.
<img width="1413" alt="Screen Shot 2023-11-05 at 9 12 23 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/bcb72c59-0e84-47a8-9edf-cba8fc0e4ce9">

## Step 3- Flask App with TailwindCSS
Using the URL and the code from class I was able to change styling and add my video.
<img width="1242" alt="Screen Shot 2023-11-05 at 6 30 59 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/98d556dd-de95-452e-bba1-1c9f50aed6ba">

## Step 4 Deploying on GCP 

Initially I was going to deploy on Azure, but then I saw that my subsciption to Azure for Students was disabled, which was not a good sign. So that is why I switched to GCP, and thankfully was able to deploy successfully.




### This is the code that I put in tailwind css
<body class="bg-white-100 font-sans">
    <header class="bg-purple-300 text-black text-center p-4">
        <h1 class="text-2xl">📎💈 Maliha's Flask App  🏘🐇 </h1>
    </header>
    <nav class="flex justify-between bg-gray-800 p-2">
        <a href="#" class="text-white px-4 py-2">Home</a>
        <a href="#" class="text-white px-4 py-2">About</a>
        <a href="#" class="text-white px-4 py-2">Services</a>
        <a href="#" class="text-white px-4 py-2">Contact</a>
    </nav>
    </div>
    <main class="p-8">
        <h2 class="text-xl mb-4">Welcome to My Flask App! </h2>

    <div class="overflow-hidden rounded-lg bg-black">
    <video controls class="h-full w-full">
        <source src="https://storage.googleapis.com/flas/video_of_black_cat%20(Original).mp4" type="video/mp4" />
        Your browser does not support the video tag.
    </video>
    </div>
   <p>This is a simple Flask app and I have imbedded a link to a video of a cat.</p>
    </main>
    <div cl
    <footer class="text-center p-4 bg-purple-300 text-white">
        <p>Copyright © 2023 My Flask App</p>
    </footer>
</body>
