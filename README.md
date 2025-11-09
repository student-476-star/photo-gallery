<h1>PROJECT 1: DESIGN OF INTERACTIVE IMAGE GALLERY</h1>


<h3>AIM:</h3>
    To design a web application for an inteactive image gallery with minimum five images.
    
<h3>DESIGN STEPS:</h3>
<h4>Step 1:</h4>
Clone the github repository and create Django admin interface.

<h4>Step 2:</h4>
Change settings.py file to allow request from all hosts.

<h4>Step 3:</h4>
Use CSS for positioning and styling.

<h4>Step 4:</h4>
Write JavaScript program for implementing interactivity.

<h4>Step 5:</h4>
Validate the HTML and CSS code.

<h4>Step 6:</h4>
Publish the website in the given URL.

<h3>PROGRAM:</h3>


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #000000;
           
        }

        h1 {
            margin-top: 20px;
            color: #f4f4f4;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 35px;
            padding: 20px;
        }

        .gallery img {
            width: 200px;
            height: 450px;
            border: 5px solid #fdeb23;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(255, 247, 247, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 7px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1> Photo Gallery</h1>
    <div class="gallery">
        <img src="image.png" alt="Image 1" onclick="openModal(this)">
        <img src="OIP.webp" alt="Image 2" onclick="openModal(this)">
        <img src="OIP (1).webp" alt="Image 3" onclick="openModal(this)">
        <img src="OIP (3).webp" alt="Image 4" onclick="openModal(this)">
        <img src="OIP (2).webp" alt="Image 5" onclick="openModal(this)">
    </div>

   
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }

        // Function to close the modal
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>
```


<h3>OUTPUT:</h3>
<img width="1920" height="1080" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/bdb0fd39-45eb-4b29-9157-c58ea32cb4c3" />
<img width="1920" height="1080" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/f8203437-c679-42b2-a818-bef9b59a0c5f" />
<img width="1920" height="1080" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/690f5398-f7b7-4215-819d-51ad5fdfa935" />






<h3>RESULT:</h3>

The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.


