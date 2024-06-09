---
license: gpl
language:
- my
---
### Hola: Multilingual-Text-Generation-(LLM) and Language-Classification-Public-Dataset
Release Date: 2/12/2024 (Myanmar Union Day)

### <b> Overview </b>
Hola dataset contains data from 11 languages, including English, Burmese, Japanese, Spanish, Chinese (Traditional), Korean, Mon, Paoh, etc. And the data was crawled from Wikipedia. Each sample is a sentence data with a label of ISO 639-1 code of respective language, e.g. en, my, ja, es, zh, ko, etc.

### <b> Data </b>
Each training sample and testing sample is a sentence data like this:
<table>
    <tr>
        <th> text </th>
    </tr>
    <tr>
        <td>
            Human evolution is the evolutionary process within the history of primates that led to the emergence of Homo sapiens as a distinct species of the hominid family, which includes all the great apes
        </td>
    </tr>
    <tr>
        <td>
            ဇီဝဗေဒ ပညာတွင် ဆင့်ကဲပြောင်းလဲမှုဖြစ်စဉ် သို့မဟုတ် အီဗော်လူးရှင်း ဆိုသည်မှာ သက်ရှိအစုအဝေးများတွင် တွေ့ရသော မျိုးရိုးလိုက်သည့် လက္ခဏာရပ်များ အချိန်နှင့် အမျှ ပြောင်းလဲသွားခြင်းကို ခေါ်ဆိုခြင်း ဖြစ်သည်
        </td>
    </tr>
    <tr>
        <td>
            人類の進化（じんるいのしんか、英: human evolution）とは、他と異なる独立した生物種としての現生人類（英名：anatomically modern humans〈意：解剖学的現代人〉、学名：Homo sapiens〈ホモ・サピエンス〉、他説では Homo sapiens sapiens ）を主題としながら、これが属する系統群（クレード）全体を見渡そうとする概念における、当該系統群が辿ってきた生物学的進化をいう
        </td>
    </tr>
    <tr>
        <td>
            La evolución humana u hominización es el proceso de evolución biológica de la especie humana desde sus ancestros hasta la actualidad
        </td>
    </tr>
    <tr>
        <td>
            人類演化过去一直指的是在旧的解剖学意义上的，根據演化學說，所做出的各種關於现代人出现的假设
        </td>
    </tr>
    <tr>
        <td>
            인류의 진화는 사람이 하나의 구분된 종으로 나타나게 되는 과정과 발전 또는 진화 과정이다
        </td>
    </tr>
</table>

Each training sample and testing sample is labeled with one of the following labels:
<table>
    <tr>
        <th> Label </th>
        <th> Description </th>
    </tr>
    <tr>
        <td> en </td>
        <td> English </td>
    </tr>
    <tr>
        <td> my </td>
        <td> Myanmar </td>
    </tr>
    <tr>
        <td> ja </td>
        <td> Japan </td>
    </tr>
    <tr>
        <td> es </td>
        <td> Spanish </td>
    </tr>
    <tr>
        <td> zh </td>
        <td> Simplified Chinese </td>
    </tr>
    <tr>
        <td> ko </td>
        <td> Korean </td>
    </tr>
    <tr>
        <td> si </td>
        <td> Sinhalese </td>
    </tr>
    <tr>
        <td> ta </td>
        <td> Tamil </td>
    </tr>
    <tr>
        <td> sw </td>
        <td> Swahili </td>
    </tr>
    <tr>
        <td> mnw </td>
        <td> Mon </td>
    </tr>
    <tr>
        <td> blk </td>
        <td> Paoh </td>
    </tr>
</table>

### How to load the dataset: 
```
from datasets import load_dataset
dataset = load_dataset("simbolo-ai/hola")
```

### Contributors:

Main Contributor: [Sa Phyo Thu Htet](https://github.com/SaPhyoThuHtet)

Other Contributors: Kaung Khant Ko Ko, Phuu Pwint Thinzar Kyaing, Yin Htwe

### How to Cite:
```bibtex
@misc{wiki-burmese-sentences,
  author = {{Sa Phyo Thu Htet}},
  title = {hola},
  url = {https://huggingface.co/datasets/simbolo-ai/hola},
  urldate = {2024-2-12},
  date = {2024-2-12}
}
```