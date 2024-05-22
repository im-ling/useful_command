# ffmpeg concat 多音频合成

ffmpeg \
-i e56c7b8d-730e-4036-bb1b-785eb7847ef5.m4a \
-i b61c6aa1-d6f9-4a10-a0fa-6a1485afc393.m4a \
-i 28a5cae2-6ca5-4604-a41d-6ffcc3fde6e0.m4a \
-i e96a9381-2775-4846-8465-e6e7b00b46ce.m4a \
-i c6f394a4-bd2a-4627-adc4-d726ffe460b0.m4a \
-i a2dd3df8-9235-4eb3-b86d-a9166dbd94c5.m4a \
-i b4ba28b4-deab-4d21-b35c-bff197125227.m4a \
-filter_complex "[0:a][1:a][2:a][3:a][4:a][5:a][6:a]concat=n=7:v=0:a=1" \
final.m4a


# ffmpeg 音频提取
ffmpeg -i 5013681767452924.mp4 -vn -acodec copy 5013681767452924.aac

# sample rate 转换
$ ffmpeg -i final.mp3 -ar 44100 final44100.mp3

# codecs 查询
ffmpeg -codecs | grep encoders 