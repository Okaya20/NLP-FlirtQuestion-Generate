# NLP-FlirtQuestion-Generate


İlk kısımı <b>Andrej Karpathy'nin</b> makemore adlı modelini esas alarak oluşturdum. Daha basit ve değiştirilebilirliği kolay.



<p>
İkinci kısımda ise biraz daha(baya) kompleks olan bir model kullanmak istedim aradaki farkı görmek için, o komplekslerin direkt yazıldığı örnekler bulamadğım için Keras kütüphanesinden yararlandım.
Bir karşılaştırma yapmak istediğim için iki modelde de multinominal bir yaklaşım uyguladım. Ancak ilk modelde şu an 3 blok aralıklarla ölçüyor,LSTM modelinde ise her kelime 1 adım ilerleyerek bağlanıyor.
  </p>
4 tane dictionary var;
<br>
<br>
-wi : word to index; kelimeleri enumerate ediyo
<br>
-iw : index to word; yukarıdakinin tersi
<br>
-nwi :new word to index +1 ;    824 kelime var bunlardan ? joker,bitirici karakter yani bu gelince durucak ben de 0 yaptım. Sorun şu ki padding işlemi(sağa kaydırma) 0 kullanıyo bu sebeple sayıyı 1 arttırdım. Sayıyı bir arttırınca index problemleriyle karşışaltım. Bir yerlerde +1 varsa çok dikkate almayın :D
<br>
-niw : new index+1 to word ; yukarıdakinin tersi
<br>
<br>
<br>
İkinci model'in train edilmesi 15-20 dakika kadar sürebilir.


Not: Read Me dosyasını daha açıkklayıcı şekilde düzenlicem.
