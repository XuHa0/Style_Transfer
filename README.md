Environment:
    python3.7
    tensorflow2.0
    Tesla P100-PCIE-16GB

Pre-trained model:
    https://github.com/fchollet/deep-learning-models/releases/download/v0.1/vgg19_weights_tf_dim_ordering_tf_kernels.h5
    https://github.com/fchollet/deep-learning-models/releases/download/v0.1/vgg19_weights_tf_dim_ordering_tf_kernels_notop.h5
 ps：运行代码的时候会自动下载加载模型需要使用VPN,没有VPN的话也可以预先将上面网址的模型下载到./keras/models目录下。仅仅第一次运行代码的时候需要下载模型，之后运行时代码会自动加载models目录底下的模型。

content_path和style_path的路径为图片的网址，可以自行修改。
代码运行的时间可能会比较长，建议使用GPU版本的tensorflow运行，在Tesla P100-PCIE-16GB下的运行时间为37.4s。

How it works
bash run.sh

content.jpg 和 style.jpg需保存在iamges目录下 输出图片保存在output目录下 也可以自行修改run.sh文件定义图片文件路径。

