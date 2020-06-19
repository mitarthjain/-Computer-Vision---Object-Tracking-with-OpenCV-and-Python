# Computer-Vision---Object-Tracking-with-OpenCV-and-Python </br>

# Tasks</br>
Optical Flow</br>
Dense Optical Flow</br>
MeanShift Tracking</br>
CamShift Tracking</br>
Single Tracking</br>
Multi Tracking</br>


Optical Flow: https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_video/py_lucas_kanade/py_lucas_kanade.html</br>

ShiTomasi: https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_feature2d/py_shi_tomasi/py_shi_tomasi.html </br>

Lucas kanade: https://en.wikipedia.org/wiki/Lucas%E2%80%93Kanade_method </br>

Gunnar Farneback's algorithm.</br>
calcOpticalFlowFarneback(prev, next, flow, pyr_scale, levels, winsize, iterations, poly_n, poly_sigma, flags) -> flow </br>

1. prev first 8-bit single-channel input image.</br>
2. next second input image of the same size and the same type as prev.</br>
3. flow computed flow image that has the same size as prev and type CV_32FC2.</br>
4. pyr_scale parameter, specifying the image scale (<1) to build pyramids for each image</br>
   4a.   pyr_scale=0.5 means a classical pyramid, where each next layer is twice smaller than the previous one.</br>
5. levels number of pyramid layers including the initial image; levels=1 means that no extra layers are created and only the original images are used.</br>
6. winsize averaging window size</br>
   6a.  larger values increase the algorithm robustness to image</br>
7. noise and give more chances for fast motion detection, but yield more blurred motion field.</br>
8. iterations number of iterations the algorithm does at each pyramid level.</br>
9. poly_n size of the pixel neighborhood used to find polynomial expansion in each pixel</br>
   9a.   larger values mean that the image will be approximated with smoother surfaces, </br>
10. yielding more robust algorithm and more blurred motion field, typically poly_n =5 or 7.</br>
11. poly_sigma standard deviation of the Gaussian that is used to smooth derivatives used as a basis for the polynomial expansion; for poly_n=5, you can set poly_sigma=1.1, for poly_n=7, a good value would be poly_sigma=1.5.</br>

Meanshift and Camshift: https://docs.opencv.org/master/d7/d00/tutorial_meanshift.html
