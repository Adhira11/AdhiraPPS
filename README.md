# AdhiraPPS
Captcha Generator 

from tkinter import Tk, Label, Entry, Button, END
from PIL import ImageTk, Image
# Import the following modules
from captcha.image import ImageCaptcha

# Create an image instance of the given size
image = ImageCaptcha(width=280, height=90)

# Image captcha text
captcha_text = 'captcha'

# Generate the image of the given text
data = image.generate(captcha_text)

# Write the image on the given file and save it
image.write(captcha_text, 'CAPTCHA.png')
