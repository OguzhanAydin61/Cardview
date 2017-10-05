# Cardview
Test project for cardview
# Projeye Veri Ekleme
prepareAlbums() metodu içinde ekleme yapılacak kısım yazılıyor.

- İstek Yönetemleri: Belirlenen retrofit yapısına göre oluyor. 
Post veya Get ile oluyor.
#Proje UI
- Burda cardview başlıklı RecyclerView Adapter kullandık. Adapter içindeki her menude :

    - Add to Favourites
    - Go to Place 

    
 *  Bizi etkileyen yerler(değişiklik yapılacak yerler):
    + Album sınıfı düzenlenecek ve bizim verilerimize göre yenilenecek
    + Adapter sınıfı içinde onBindViewHolder() metodu içinde resim alma formatı değişiklik gösterebilir retrofit kullanmınıa göre
    
    +   showPopupMenu() metodu içinde alt tarafta yer alacak carviewler içindeki popup menü içindeki seçeneklerin eventları yer alıyor setOnMenuItemClickListener() içinin tasarıma göre tekrardan yazılması lazım.
        
         - (Not: Listener eventı->MyMenuItemClickListener() içine implemente olmuş yani click olayları için burasının içerisi düzenlenecek!)
                
               -RecyclerView mantığını daha iyi anlamak için:   
                    
             -    [https://developer.android.com/reference/android/support/v7/widget/RecyclerView.html] 
                  
             - [https://www.youtube.com/watch?v=USbTcGx1mD0&list=PLk7v1Z2rk4hjHrGKo9GqOtLs1e2bglHHA ]   
      
    + MainActivity içinde prepareAlbums() kısmında adaptere veri ekleme işini yapıyoruz.
    
    + Son olarak MainActivity içinde küçük cardviewlerin poziyson ve dizaynını değiştirmek için getItemOffsets() içinde oynama yapmalıyız.
                      
                  NOT: Araç çubuğu genişletilip daraltıldığında başlık gizleme ve gösterilme işlevini düzenlemek için initCollapsingToolbar() metodunda değişiklik yapıyoruz.    
        
    
  