Instructions - 
reverse_compression.py generates an noisy image with an stencil image hidden in the noise.
to use, replace/edit stencil.png to whatever image you want to hide in the noise. it must be a b/w image
afterwards run the reverse compression.py file. it will prompt you for desired rgb values for noise and hidden image. these should be similar but different.
you can experiment if you want. i found that (128,128,128) for the noise and (200,128,128) for the signal works well. i use 5 as the buffer value.
everything else is just follow the prompts.
the output image will be saved as noise.png in the root folder

to reveal the stencil image-
use an image software that supports low complexity bilinear compression. i use paint.net. compress by 50% with bilinear (low quality), with gamma correction turned off.