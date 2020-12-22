import pyttsx3
import PyPDF2
book = open('b.pdf','rb')
pdf = PyPDF2.PdfFileReader(book)
pages = pdf.numPages
print(pages)
sr = pyttsx3.init()
for num in range(0,pages):
    page = pdf.getPage(0)
    text = page.extractText()
    sr.say(text)
    sr.runAndWait()
