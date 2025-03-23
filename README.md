# Enformer
Simple Enformer website deployment using onnx and tfjs, currently still subject to improvements.

If you want to see the changes I made for the Enformer model, repo is here: https://github.com/peterguzw0927/Enformer_new

** Please make sure the input sequence have 196608 length**

If you have costumized enformer you can convert onnx file to tf model and then to tfjs model using:

convert to tf: (convertenv2) onnx-tf convert -i test_enformer.onnx -o tf_model

convert to tfjs: (convertenv3) tensorflowjs_converter tf_model/ tfjs_model/ --input_format tf_saved_model --output_format tfjs_graph_model --quantize_uint8


Access here: [https://peterguzw0927.github.io/Enformer/](https://peterguzw0927.github.io/Enformer.github.io/)
