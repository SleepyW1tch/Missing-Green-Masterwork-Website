Readme file

URL​: https://pitch-salact.vercel.app/

Topic description​: 
I created this website as part of my IxD MA masterwork, I intended to use it as a summary/base for documentation and knowledge-sharing. Some materials can be found related to the user flows of this educational game.
The topic of my masterwork is educating young people about greenwashing, its usual behavihours and buzzwords, etc.

Source of codes​:
ChatGPT, occasional help from senior developer, and lectures.

Source of images​:
The photos were taken by me.
Logo and visual design created by me.
Tree icon: https://www.flaticon.com/free-icon/tree_12414749?term=pixel&page=1&position=23&origin=tag&related_id=12414749 
Pitch-salact Start mini picture: generated with ChatGPT. (assets -> start proto) 
3D model for heart tokens: https://www.printables.com/model/1070917-heart-token/files 

What kind of js code did you use​:
 <script>
        const btnUp = {
          el: document.querySelector(".btn-up"),
          show() {
            this.el.classList.remove("btn-up_hide");
          },
          hide() {
            this.el.classList.add("btn-up_hide");
          },
          addEventListener() {
            window.addEventListener("scroll", () => {
              const scrollY =
                window.scrollY || document.documentElement.scrollTop;
              scrollY > 400 ? this.show() : this.hide();
            });
            document.querySelector(".btn-up").onclick = () => {
              window.scrollTo({
                top: 0,
                left: 0,
                behavior: "smooth",
              });
            };
          },
        };
  
        btnUp.addEventListener();
      </script>

       <script>
    let lastClicked = null;

    function toggleImage(element) {
      const img = element.querySelector('img');
      
      // Check if the clicked image is the same as the last clicked image
      if (lastClicked === img) {
        // If it's the same image, reset it back to original size
        img.style.transform = 'scale(1)';
        lastClicked = null;
      } else {
        // Otherwise, scale it up to full size
        if (lastClicked) {
          // Reset the previous image if there was one
          lastClicked.style.transform = 'scale(1)';
        }
        img.style.transform = 'scale(2)'; // Scale up the clicked image
        lastClicked = img;
      }
    }

    // Function to open the modal with the clicked image
function openModal(imgElement) {
  const modal = document.getElementById("image-modal");
  const modalImage = document.getElementById("modal-image");
  
  // Set the src of the modal image to the clicked image's src
  modalImage.src = imgElement.src;
  
  // Show the modal
  modal.style.display = "block";
}

// Function to close the modal
function closeModal() {
  const modal = document.getElementById("image-modal");
  modal.style.display = "none";
}

  </script>
  

What kind of font did you use​:
https://fonts.google.com/specimen/Press+Start+2P
https://fonts.google.com/specimen/Bricolage+Grotesque

Your name:
Emese Kata Hubert
