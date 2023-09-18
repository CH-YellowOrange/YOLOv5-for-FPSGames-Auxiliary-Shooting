
# Self-aiming of FPS shooting game based on YOLOv5

# Statement:
- This project is only for learning and communication and cannot be used for commercial purposes or for illegal purposes (including but not limited to: use for making game plug-ins, etc.).
- I have nothing to do with any consequences of using this project!
- By using this project, you agree to this statement by default!

  
# introduction
 -  This project is based on yolov5 and implements the self-aiming AI of an FPS game (CSGO, CrossFire, etc.).
   
 -  But it cannot be used for illegal purposes! ! !
 -  But it cannot be used for illegal purposes! ! !
 -  But it cannot be used for illegal purposes! ! !
   
 -  The pre-trained model is based on [CSGO](https://store.steampowered.com/app/730/CounterStrike_Global_Offensive). 

# Training
  
  > - Please refer to [yolov5](https://github.com/ultralytics/yolov5).

# How to use?
  > - Before starting, modify the screen resolution, detection frame range and other parameters in the '''utils/FPSUtils.py''' file.
  > - Please modify the model location in the '''FPSdetect.py''' file: '''model = attempt_load('Change here to your own path\FPSAutomaticAiming\yolov5s.pt', map_location=device) '''.
  > - Modify the mouse movement related code in '''Main.py''' to your own mouse movement code.
  > - After modifying the relevant parameters, run '''`Main.py''' directly to start this project.


# Environment configuration
 
  Use conda to import ```yolo.yaml```。
  ```
  name: yolo
channels:
  - pytorch
  - conda-forge
  - https://mirrors.ustc.edu.cn/anaconda/pkgs/main
  - https://mirrors.ustc.edu.cn/anaconda/pkgs/free
  - https://mirrors.bfsu.edu.cn/anaconda/pkgs/msys2
  - https://mirrors.bfsu.edu.cn/anaconda/pkgs/pro
  - https://mirrors.bfsu.edu.cn/anaconda/pkgs/r
  - https://mirrors.bfsu.edu.cn/anaconda/pkgs/free
  - https://mirrors.bfsu.edu.cn/anaconda/pkgs/main
  - defaults
dependencies:
  - absl-py=0.13.0=py38haa95532_0
  - aiohttp=3.7.4=py38h2bbff1b_1
  - async-timeout=3.0.1=py38haa95532_0
  - attrs=21.2.0=pyhd3eb1b0_0
  - blas=1.0=mkl
  - blinker=1.4=py38haa95532_0
  - bottleneck=1.3.2=py38h2a96729_1
  - brotli=1.0.9=ha925a31_2
  - brotlipy=0.7.0=py38h2bbff1b_1003
  - ca-certificates=2021.5.30=h5b45459_0
  - cachetools=4.2.2=pyhd3eb1b0_0
  - certifi=2021.5.30=py38haa244fe_0
  - cffi=1.14.6=py38h2bbff1b_0
  - chardet=3.0.4=py38haa95532_1003
  - click=8.0.1=pyhd3eb1b0_0
  - cryptography=3.4.7=py38h71e12ea_0
  - cudatoolkit=10.2.89=h74a9793_1
  - cycler=0.10.0=py38_0
  - fonttools=4.25.0=pyhd3eb1b0_0
  - freetype=2.10.4=hd328e21_0
  - google-auth=1.33.0=pyhd3eb1b0_0
  - google-auth-oauthlib=0.4.1=py_2
  - grpcio=1.35.0=py38hc60d5dd_0
  - icc_rt=2019.0.0=h0cc432a_1
  - icu=58.2=ha925a31_3
  - idna=2.10=pyhd3eb1b0_0
  - importlib-metadata=3.10.0=py38haa95532_0
  - intel-openmp=2021.3.0=haa95532_3372
  - jpeg=9b=hb83a4c4_2
  - kiwisolver=1.3.1=py38hd77b12b_0
  - libpng=1.6.37=h2a8f88b_0
  - libprotobuf=3.17.2=h23ce68f_1
  - libtiff=4.2.0=hd0e1b90_0
  - libuv=1.40.0=he774522_0
  - lz4-c=1.9.3=h2bbff1b_1
  - markdown=3.3.4=py38haa95532_0
  - matplotlib=3.4.2=py38haa95532_0
  - matplotlib-base=3.4.2=py38h49ac443_0
  - mkl=2021.3.0=haa95532_524
  - mkl-service=2.4.0=py38h2bbff1b_0
  - mkl_fft=1.3.0=py38h277e83a_2
  - mkl_random=1.2.2=py38hf11a4ad_0
  - msys2-conda-epoch=20160418=1
  - multidict=5.1.0=py38h2bbff1b_2
  - munkres=1.1.4=py_0
  - ninja=1.7.2=0
  - numexpr=2.7.3=py38hb80d3ca_1
  - numpy=1.20.3=py38ha4e8547_0
  - numpy-base=1.20.3=py38hc2deb75_0
  - oauthlib=3.1.1=pyhd3eb1b0_0
  - olefile=0.46=py_0
  - openssl=1.1.1k=h8ffe710_1
  - pandas=1.3.1=py38h6214cd6_0
  - pillow=8.3.1=py38h4fa10fc_0
  - pip=21.0.1=py38haa95532_0
  - protobuf=3.17.2=py38hd77b12b_0
  - pyasn1=0.4.8=py_0
  - pyasn1-modules=0.2.8=py_0
  - pycparser=2.20=py_2
  - pyjwt=2.1.0=py38haa95532_0
  - pyopenssl=20.0.1=pyhd3eb1b0_1
  - pyparsing=2.4.7=pyhd3eb1b0_0
  - pyqt=5.9.2=py38ha925a31_4
  - pysocks=1.7.1=py38haa95532_0
  - python=3.8.11=h6244533_1
  - python-dateutil=2.8.2=pyhd3eb1b0_0
  - python-mss=6.1.0=pyhd3deb0d_0
  - python_abi=3.8=2_cp38
  - pytorch=1.9.0=py3.8_cuda10.2_cudnn7_0
  - pytz=2021.1=pyhd3eb1b0_0
  - pyyaml=5.4.1=py38h2bbff1b_1
  - qt=5.9.7=vc14h73c81de_0
  - requests=2.25.1=pyhd3eb1b0_0
  - requests-oauthlib=1.3.0=py_0
  - rsa=4.7.2=pyhd3eb1b0_1
  - scipy=1.6.2=py38h66253e8_1
  - seaborn=0.11.2=pyhd3eb1b0_0
  - setuptools=52.0.0=py38haa95532_0
  - sip=4.19.13=py38ha925a31_0
  - six=1.16.0=pyhd3eb1b0_0
  - sqlite=3.36.0=h2bbff1b_0
  - tensorboard=2.5.0=py_0
  - tensorboard-plugin-wit=1.6.0=py_0
  - tk=8.6.10=he774522_0
  - torchaudio=0.9.0=py38
  - torchvision=0.10.0=py38_cu102
  - tornado=6.1=py38h2bbff1b_0
  - tqdm=4.62.1=pyhd3eb1b0_1
  - typing-extensions=3.10.0.0=hd3eb1b0_0
  - typing_extensions=3.10.0.0=pyh06a4308_0
  - urllib3=1.26.6=pyhd3eb1b0_1
  - vc=14.2=h21ff451_1
  - vs2015_runtime=14.27.29016=h5e58377_2
  - werkzeug=1.0.1=pyhd3eb1b0_0
  - wheel=0.37.0=pyhd3eb1b0_0
  - win_inet_pton=1.1.0=py38haa95532_0
  - wincertstore=0.2=py38_0
  - xz=5.2.5=h62dcd97_0
  - yaml=0.2.5=he774522_0
  - yarl=1.6.3=py38h2bbff1b_0
  - zipp=3.5.0=pyhd3eb1b0_0
  - zlib=1.2.11=h62dcd97_4
  - zstd=1.4.9=h19a0ad4_0
  - pip:
    - colorama==0.4.4
    - mouseinfo==0.1.3
    - opencv-python==4.5.3.56
    - polygon3==3.0.9.1
    - pyautogui==0.9.53
    - pygetwindow==0.0.9
    - pymsgbox==1.0.9
    - pyperclip==1.8.2
    - pyrect==0.1.4
    - pyscreeze==0.1.27
    - pytweening==1.0.3
    - tensorboard-data-server==0.6.1
    - thop==0.0.31-2005241907

