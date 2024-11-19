# A manga auto-translation framework based on manga-ocr and paddleOCR
This is a framework designed for text detection and recognition in black-and-white Japanese manga. It utilizes PaddleOCR for text detection and manga-ocr for text recognition, enabling seamless identification of Japanese text in manga. With a single click, it translates the original Japanese text into Chinese and automatically fills the translated text into the corresponding positions within the manga panels.

## Fine-tuning
We fine-tuned the ch_PP-OCRv4_server_det model in PaddleOCR using [Manga109-s](http://www.manga109.org/en/download_s.html) to achieve improved text detection performance. We directly use the pre-trained [manga-ocr](https://github.com/kha-white/manga-ocr) model for text recognition.

## Requirements
Environment Requirements for [manga-ocr](https://github.com/kha-white/manga-ocr)


Environment Requirements and [Documentation](https://paddlepaddle.github.io/PaddleOCR/latest/) for [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)

## Running project
After setting up the required environment, simply modify the source image path and the output image path in the `get_translated_image.py` file. Then, run the `main` function to convert Japanese text in black-and-white manga into Chinese effortlessly.

## Results Demonstration
| Original  | Translated |
| ------------- | ------------- |
| ![original manga](https://github.com/HUA-Python/manga_ocr_translator/blob/master/example_pic/t8.jpg)  | ![translated manga](https://github.com/HUA-Python/manga_ocr_translator/blob/master/example_pic/t8_translated.jpg)  |

### PS
The Japanese translation used in this framework is inaccurate and unstable. You can replace the translation part with a more stable translation API in the `get_translated_image.py` file, as needed.
