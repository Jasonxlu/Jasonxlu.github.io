---
layout: page
title: Resume
image: assets/images/purple.jpeg
description: An overview of my experience.
nav-menu: true
---

<style>
    .center {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 75%;
        margin-top: 50px;
        margin-bottom: 25px;
        padding-right: 25px;
        padding-left: 25px; 
        padding-top: 25px;
        padding-bottom: 25px;
        max-width: 75%;
        height: auto;
    }

    #resume {
        cursor: pointer;
        transition: 0.3s;
        box-shadow: 0px 6px 8px 0 rgba(0, 0, 0, 0.2), 0px 8px 20px 0 rgba(0, 0, 0, 0.19);
    }

    #resume:hover {
        opacity: 0.7;
    }

    /* Creating Modal Overlay */
    .modal {
        display: none;
        position: fixed;
        z-index: 2;
        padding-top: 100px;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        overflow: auto;
        background-color: rgb(0,0,0);
        background-color: rgba(0,0,0,0.9);
    }

    /* Content of the modal */
    .modal-content {
        margin: auto;
        display: block;
        width: 80%;
        max-width: 700px;
    }

    /* Modal Image Caption */
    #caption {
        margin: auto;
        display: block;
        width: 80%;
        max-width: 700px;
        text-align: center;
        color: #ccc;
        padding: 10px 0;
        height: 150px;
    }

    /* Animation (Find in _image.scss file) */
    .modal-content, #caption {
        animation-name: zoom;
        animation duration: 0.6s;
    }

    @keyframes zoom {
        from {transform: scale(0.1)}
        to {transform: scale(1)}
    }

    /* Close button */
    .close {
        position: absolute;
        top: 50px;
        right: 35px;
        color: #f1f1f1;
        font-size: 40px;
        font-weight: bold;
        transition: 0.3s;
    }

    .close:hover, .close:focus {
        color: #bbb;
        text-decoration: none;
        cursor: pointer;
    }

    /* Mobile responsive */
    @media only screen and (max-width: 700px) {
        .modal-content {
            width: 100%;
        }
    }

</style>

<img class="center" id="resume" src="assets/images/Resume.jpg" alt="Last updated: 9/4/2022">

<!-- Modal  -->
<div id="resumeModal" class="modal"> 
    <span class="close">&times;</span>
    <img class="modal-content" id="modalimg">
    <div id="caption"></div>
</div>

<div class="content">
    <div class="inner">
            <a href="assets/Resume.pdf" class="button special icon fa-download" target="_blank" rel="noopener noreferrer" download="Resume">Download</a>
    </div>
</div>

<script>
    var modal = document.getElementById("resumeModal");
    var img = document.getElementById("resume");
    var modalImg = document.getElementById("modalimg");
    var captionText = document.getElementById("caption");
    img.onclick = function()
    {
        modal.style.display = "inline-block";
        modalImg.src = this.src;
        captionText.innerHTML = this.alt;
    }

    var span = document.getElementsByClassName("close")[0];

    // Closing the modal
    document.addEventListener('keydown', function(event) {
    if(event.keyCode == 27) {
        modal.style.display = "none";
    }});

    span.onclick = function()
    {
        modal.style.display = "none";
    }

    
</script>
