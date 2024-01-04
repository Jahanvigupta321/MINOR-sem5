Secured Palette is a web application developed using Streamlit in Python, aiming to enhance
information security through a combination of LSB (Least Significant Bit) steganography and visual
cryptography techniques. In the encoding phase, the application takes an input image and text to be
concealed. LSB steganography involves subtly adjusting the least significant bits of colored pixels
in the image, embedding the text message within the image without perceptible alterations.

Following the steganographic process, visual cryptography is employed. The encoded image is
divided into two shares using visual cryptography. Each share independently reveals no information
about the original image or message, but when superimposed, the visual cryptography mechanism
reconstructs the original image, making it visually perceptible. This process ensures that neither
share alone discloses any sensitive information.

For decoding, the web application prompts the user to upload the shares of the visual cryptography
scheme. Upon overlap, the shares reconstruct the hidden image. Internally, LSB steganography is
applied again to extract the concealed text message from the reconstructed image. This dual-layered
security approach combines the obscurity of LSB steganography with the cryptographic resilience
of visual cryptography, providing a robust means of safeguarding secrets. The innovative fusion of
these techniques fortifies data protection by making it challenging for unauthorized entities to
discern both the existence of concealed information and its content.
