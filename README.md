# Stego-Cryptography

### 👋 Introduction 

This project uses encryption and steganography methods in a form of parallel computing to hide a secret image/text file in a cover image, and send it across mediums. It is an effective method of protecting data by hashing the secret text/image using encryption, hiding it with steganography, and passing it through various mediums until it reaches it's destination. In general, Stego-cryptography is incredibly useful for data security and privacy, and espionage! 

However, this method has had it's slight flaws as performing such a heavy computation on hundreds of texts or images can be time and space consuming. Our program deals with the same using parallel computing to greatly reduce time and space consumption. 
To show the difference between serialized and threaded stego-crytpography, we create visualizations 


---
### 📖 Historical Value

Dating back to the 5th century BC, steganography is one of the oldest methods of concealing secret information. According to the classical author Herodotus, it was first used by the tyrant Histiaeus, who shaved the head of a servant before tattooing a message on the poor man's scalp! Steganography has found it's worth in Cold War, Nazi Germany, RAW's stealth missions among many uses. Cryptography has become more prevalent in recent times due to the introduction of Blockchain and cryptocurrencies.

---
### 📋 How to Run

- Install the latest version of [PyCharm](https://www.jetbrains.com/help/pycharm/installation-guide.html) and [Python 3](https://www.python.org/downloads/).
- NOTE: You can use any other IDE or editor, PyCharm is recommended as it supports most of the libraries used in this project. 
- Open the project in PyCharm IDE  and install the dependencies and libraries necessary.
- Open the directories Stego-Cryptography/big and Stego-Cryptography/small. These consist of cover(big) and secret(small) images (in terms of size in kB).
- Change the directories of the big and small folders in the following file(s) to their directories in your local system=>
      a. ```imagestegserial.py```: image embed in image steganography using serialization
      b. ```imagestegthread.py```: image embed in image steganography using parallelization
      c. ```pureTextstegencodeparallel.py```: text embed in image steganography using parallelization
      d. ```pureTextstegs.py```: text embed in image steganography using serialization 
- Run any of the above files using their driver codes to a) Encrypt or b) Decrypt image/text file(s).

(Important thing to note is that the individual size of a cover image always surpasses that of a secret image or text file.)

---

### 📈 Observations

The maximum sample size of cover/secret images was chosen to be 15, as the process takes considerable computation. Comparisons can be drawn by choosing more, or less images. 
- **Image Steganography**:
  a. Serially encoding 15 secret images in 15 cover images:
  
  ![image](https://user-images.githubusercontent.com/55179780/190957806-a39f3231-e808-4fd3-a5c6-c257180ebe6d.png)

  b. Parallelly encoding 15 secret images in 15 cover images:
  
  ![image](https://user-images.githubusercontent.com/55179780/190957916-d03fc6d8-1882-4519-bc0f-a4d4961cb819.png)

  c. Serially decoding 15 images:
  
  ![image](https://user-images.githubusercontent.com/55179780/190957970-65e03b3a-c471-4919-a787-eb6ce25e1c35.png)

  d. Parallelly decoding 15 images:
  
  ![image](https://user-images.githubusercontent.com/55179780/190958488-edbdcf26-6568-48fa-8bb3-6730d5367488.png)

- **Text Steganography**:
  a. Serial Encoding of a text file in 15 cover images:
  
  ![image](https://user-images.githubusercontent.com/55179780/190958716-9dba7cb0-beef-45a9-be12-dbdb20ec3d39.png)

  b. Parallel Encoding of a text file in 15 cover images:
  
  ![image](https://user-images.githubusercontent.com/55179780/190958711-fd985f09-0635-4ef9-8230-124f3795bce3.png)
  
  c. Serial Decoding time:
  
  ![image](https://user-images.githubusercontent.com/55179780/190958793-9a875bb9-86a4-4d9e-8ce8-5980f147bdf0.png)

  d. Parallel Decoding time:
  
  ![image](https://user-images.githubusercontent.com/55179780/190958848-834fb3e5-4050-40ee-b206-acd6cb3417c3.png)
  
 - **Results**
 
      a. Image Steganography:
      
      <img src="https://user-images.githubusercontent.com/55179780/190960395-382af15c-d703-456b-9ff4-e68be55df75a.png" alt="big_cover" height="60" width="60" /> + <img src = "https://user-images.githubusercontent.com/55179780/190960427-1748007b-095a-4695-89e8-d52e7cda2cef.png" alt="small_hidden" height="60" width="60"/>  <====> <img src="https://user-images.githubusercontent.com/55179780/190960074-b5335e2a-fa63-4446-bbe8-91c6c75924f1.png" alt="output" width="60" height="60"/>

      NOTE: Open the output image to see the changes. the background of cover img in this example is heavily contrasting to the hidden img, hence being rather visible. It is usually not the case and is solely used to serve as an example.
      
      b. Text steganography:
      
      <img src="https://user-images.githubusercontent.com/55179780/190961682-aeaf9332-c176-4227-ba76-30e96b83a97c.png" alt="hidden.txt" height="60" width="60"/> + <img src="https://user-images.githubusercontent.com/55179780/190962159-0c256176-d35e-4d0e-9996-8711969b28d4.png" alt="small_cover" height="60" width="60"/> <=====> <img src="https://user-images.githubusercontent.com/55179780/190961986-ce7eb615-3671-4284-afe0-d87a297f038e.png" alt ="output" height="60" width="60"/>

---

### 🔮 Future Work

FrontEnd, Cloud DataBase connectivity, deployment as a web application. More updates to the algorithm, shorten time complexity.

---

### 🧰 ToolKit


<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="python" width="50" height="50" /> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" alt="PyCharm" width="50" height="50" /> 

---
