OpenAI recently announced the creation of a cipher watermark to detect whether a particular piece of content was generated using the GPT language model. I became interested in exploring how such a cipher could be implemented without sacrificing its effectiveness through formatting.

There are several methods for creating a cipher watermark that can be used to hide secret messages or signatures within text. One notable method is text formatting, such as FontCode. However, this method can be eliminated as a candidate for large language model generated content watermark if the formatting is changed. Another method is the use of zero-width characters, which are characters that are not visible but still present in the text. However, not all zero-width characters are suitable for use as a cipher watermark. After conducting research, I discovered that only the zero-width character [ALT]+0160, which is essentially a "invisible space," can be used as a cipher watermark for large language models. This is because it is not detectable by any text or code editors, making it a perfect cipher-based watermark.

### Reference:
<ul>
<li>https://www.newscientist.com/article/2350655-openai-is-developing-a-watermark-to-identify-work-from-its-gpt-text-ai/</li>
<li>https://www.cs.columbia.edu/cg/fontcode/</li>
<li>https://en.wikipedia.org/wiki/Zero-width_space</li>
</ul>
