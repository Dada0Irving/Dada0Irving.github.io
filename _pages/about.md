---
permalink: /
title: "Welcome to Owen's website!"
excerpt: "Owen"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<!-- Wrapper for iframe with loading overlay -->
<div style="position: relative; width: 100%; height: 650px;">

    <!-- Loading Overlay -->
    <div id="loading-overlay" 
         style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; 
                background-color: white; color: black; 
                display: flex; justify-content: center; align-items: center; 
                font-size: 24px; font-weight: bold; z-index: 2;">
        Loading Virtual Owen...
    </div>

    <!-- The iframe -->
    <iframe id="virtual-owen" 
            src="https://virtual-owen-0033e3bcabb0.herokuapp.com/" 
            width="100%" height="650px" 
            style="border: none; position: absolute; top: 0; left: 0; z-index: 1;"></iframe>
</div>

<!-- Optional: JavaScript to remove overlay after iframe loads -->
<script>
    window.addEventListener('load', function() {
        const iframe = document.getElementById('virtual-owen');
        const loadingOverlay = document.getElementById('loading-overlay');

        iframe.onload = function() {
            loadingOverlay.style.display = 'none';  // Hide the overlay when iframe is loaded
        };

        // Optional: Fallback to hide the overlay after 5 seconds if iframe takes too long
        setTimeout(() => loadingOverlay.style.display = 'none', 5000);
    });
</script>

**I am currently seeking HCI-related PhD positions for Fall 2025.**
