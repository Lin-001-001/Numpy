# 运行环境
运行 python -m pip install -r requirements.txt
# 编程内容
TODO-01 ~ TODO-06
# 如何复现
1. 编译 image_encoder.py.
2. 运行 run.py, 结果存储在 output_tokens.npz
3. 运行 check.py，在控制台检验结果。
# 详细 output_tokens
在终端输入以下信息
1. python
2. import numpy as np
3. ref = np.load("./assets/reference_outputs.npz')
4. ref = dict(ref)
5. ref_output = ref['output_tokens']
6. mine = np.load('output_tokens.npz')
7. mine = dict(mine)
8. output = ref['output_tokens']
9. output
10. np.round(output, ref_output)
