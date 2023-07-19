# Car plate recognize system

The project is a web app used for license plate recognition, powered by a pre-trained detection ONNX model,  character and color recognition ONNX model and [EasyOCR](https://github.com/JaidedAI/EasyOCR).

The **features** of the app including multi-language support including Chinese, English and Vietnamese. Also, as color represents the type of a car in china, for example green is the new energy plate, our model is able to recognise not only the plate number but also the plate color as the example shown below. 

<img src="https://github.com/Dukeee1999/comp5405/assets/62459234/b07cf324-1c9b-4dca-9aae-49d6284a6731" alt="截屏2023-05-12 下午2.47.40" style="zoom:15%;" />
														              
                            Figure 1:  Character and plate color recognition



Besides that, our model is able to detect double-row plates such as Chinese moto plates and most of Vietnamese plate. You can see from the image belwo.

<img width="1136" alt="截屏2023-05-12 下午2 44 27" src="https://github.com/Dukeee1999/comp5405/assets/62459234/66eeb81a-9d65-4c78-af4a-a2a34bf0e2b3">

                            Figure 2 : Double-row plate recognition



Then, we can detect multi-plates in a single image at the same time. 

<img width="1134" alt="截屏2023-05-12 下午2 46 35" src="https://github.com/Dukeee1999/comp5405/assets/62459234/4ef5bc39-551d-4bff-9523-2cd1c58ddcd5">

                            Figure 3: Mutli-plates detection and recognition



Finally, I can detect cars with special characters in it such as space, dash, dot and so on.

<img width="1129" alt="截屏2023-05-12 下午2 56 12" src="https://github.com/Dukeee1999/comp5405/assets/62459234/2875cff7-e244-44d3-9fde-3ab2928dbb7b">
								 
                            Figure 4: Special character recognition



## Table of contents

[1. How to use]()

[2. Abstract]()

[3. License Plate Detection]()

[5. Character and Color Recognition]()

[6. Conclusion]()



## How to use

##### Step 1: 

Install all required packages listed by running 

```python
pip install -r requirements.txt

pip install git+https://github.com/JaidedAI/EasyOCR.git

conda install onnxruntime -c conda-forge

```

##### Step 2:

Start the flask backend by running

```python
flask run
```

and then you are able to access the web app via http://localhost:5000/ 

##### Step 3:

You can now see our welcome page and start upload images for plate detection !



## Abstract



## License Plate Detection


![PR_curve](https://github.com/Dukeee1999/comp5405/assets/62459234/744ddbbb-3b66-43e3-98f2-390dd5f6369b)

![results](https://github.com/Dukeee1999/comp5405/assets/62459234/c65b3137-49aa-488d-9ae2-cf2a46ee8823)


## Character and Color Recognition

##### CRNN color plate recognition



##### EasyOCR



## Conclusion



## References

- https://github.com/Sierkinhane/CRNN_Chinese_Characters_Rec
- https://github.com/meijieru/crnn.pytorch
- https://github.com/we0091234/crnn_plate_recognition/tree/plate_color
- https://github.com/mrzaizai2k/License-Plate-Recognition-YOLOv7-and-CNN

