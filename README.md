# KKOAla

### KKoAla: large language model for korean finance (Polyglot-12.8B based)

<p align="center">
<a href=""><img src="src/imgs/koala.PNG" width="30%"></a>
</p>

### Models

[2023/05/26] v1 버전 : Polyglot-12.8B Base, KoAlpaca, Financial Q&A Fine-tuning




| Model                    | Vol | Base | Dataset |                    Huggingface                   |
| :----------------------- | :------: | :--------------------: | :----------------: | :----------------------------------------------------------: |
| KKoAla-13B-v1         | 26G  |      Polyglot-12.8B      |        KoAlpaca + Financial Q&A        | [Huggingface Link](https://huggingface.co/mssongit/Koala-12.8b-v1)|


## Use

~~~
pip install -U torch transformers tokenizers accelerate
~~~

~~~
import torch
from transformers import pipeline, AutoModelForCausalLM

MODEL = "mssongit/Koala-12.8b-v1"
model = AutoModelForCausalLM.from_pretrained(
    MODEL,
    torch_dtype=torch.float16,
)
~~~



## Example

![image](https://github.com/mssongit/KKOAla/assets/95903180/869efec4-0653-4f88-922e-59b7a7412ad0)
