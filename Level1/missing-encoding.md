## Missing Encoding
### Challenge: Retrieve the photo of Bjoern's cat in "melee combat-mode".

Log in as user (create if not user yet). From side menu, navigate to `Photo Wall`. There will be 3 photos with the first photo with a broken link `😼 #zatschi #whoneedsfourlegs`

To see the absolute link for image with broken link, right click the broken link using Chrome browser > `Inspect` > `Elements` and see that it is 

```
assets/public/images/uploads/😼-#zatschi-#whoneedsfourlegs-1572600969477.jpg
```

If you encode the characters 
```
😼-#zatschi-#whoneedsfourlegs-1572600969477.jpg
```

you will get 
```
%F0%9F%98%BC-%23zatschi-%23whoneedsfourlegs-1572600969477.jpg
```

We now know the absolute path of the image, navigate to `http://192.168.247.136:3000/assets/public/images/uploads/%F0%9F%98%BC-%23zatschi-%23whoneedsfourlegs-1572600969477.jpg` to complete this challenge

_Note: We can observe requests from client to server using Chrome developer tools `Network`. If we filter the recorded requests by clicking `img` to we can see one of the image url requested was `http://192.168.247.136:3000/assets/public/images/uploads/%F0%9F%98%BC-` which is actually the "half encoded" url of the cat image. It is revealing that the `#` character was not being encoded thus the image was not found_