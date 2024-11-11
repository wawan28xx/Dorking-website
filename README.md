# Dorking-website


**Berikut adalah pengelompokan dorking dari daftar yang diberikan, berdasarkan kerentanannya:**

**1. SQL Injection** <br/>
Dorking SQL Injection biasanya memanfaatkan parameter pada URL yang rentan terhadap injeksi SQL. Tujuannya adalah untuk mengeksekusi perintah SQL berbahaya, seperti membaca atau mengubah data di basis data.<br/>
Contoh dork untuk SQL Injection:<br/>

*inurl:index.php?id=<br/>
inurl:article.php?ID=<br/>
inurl:newsDetail.php?id=<br/>
inurl:games.php?id=<br/>
inurl:product-item.php?id=<br/>
inurl:productdetail.php?id=<br/>
intext:"error in your SQL syntax" +site:mm<br/>
intext:"mysql_num_rows()" +site:mm<br/>
intext:"mysql_fetch_array()" +site:mm<br/>*

**2. XSS (Cross-Site Scripting)** <br/>
Dorking XSS memanfaatkan input yang tidak divalidasi dengan benar, memungkinkan injeksi kode JavaScript yang bisa dieksekusi oleh pengguna lain.<br/>
Beberapa dork yang sering dimanfaatkan untuk menemukan kerentanan XSS:<br/>
*inurl:page.php?file=<br/>
inurl:loadpsb.php?id=<br/>
inurl:rub.php?idr=<br/>
inurl:announce.php?id=<br/>*

**3. File Inclusion** <br/>
File Inclusion (LFI atau RFI) memungkinkan penyerang untuk memasukkan file dari server lain atau dari sistem lokal, untuk mengeksekusi kode dari file tersebut. Dorking ini sering digunakan untuk mencari parameter URL yang rentan terhadap teknik ini.<br/>
Contoh dork:<br/>
*inurl:loadpsb.php?id=<br/>
inurl:page.php?file=<br/>
inurl:clanek.php4?id=<br/>*

**4. Error Disclosure** <br/>
Error disclosure memungkinkan penyerang melihat pesan kesalahan yang mungkin mengandung informasi sensitif tentang server atau database yang digunakan.<br/>
Beberapa dork untuk mencari error disclosure:<br/>
*intext:"Warning: mysql_fetch_array()"
intext:"Warning: session_start()"
intext:"Warning: mysql_num_rows()"
intext:"Warning: mysql_query()"
intext:"Warning: getimagesize()"
intext:"error in your SQL syntax" +site:mm*

**5. Path Traversal**<br/>
Path Traversal memungkinkan penyerang untuk mengakses file atau direktori yang seharusnya tidak dapat diakses, dengan cara memasukkan karakter ".." dalam URL.<br/>
<br/>Contoh dork:<br/>
*inurl:showimg.php?id=<br/>
inurl:rub.php?idr<br/>*

**6. Misconfiguration dan Lainnya**<br/>
Dorking ini memanfaatkan kesalahan konfigurasi server atau aplikasi yang dapat memberikan akses yang tidak semestinya pada penyerang.<br/>
Contoh dork:<br/>
*intext:"Server Error in '/' Application"<br/>
intext:"Microsoft OLE DB Provider for ODBC Drivers error"<br/>
intext:"Invalid Querystring"<br/>
intext:"JET Database"<br/>*

**7. Information Disclosure**<br/>
Dorking ini sering digunakan untuk menemukan informasi sensitif yang tidak diproteksi dengan baik, seperti data login, konfigurasi aplikasi, dan struktur basis data.<br/>
Contoh dork:<br/>

*intext:"ADODB.Field"<br/>
intext:"BOF or EOF"<br/>
intext:"ADODB.Command"<br/>
intext:"mysql_fetch_object()"<br/>*

Setiap kategori kerentanan ini memiliki teknik eksploitasi dan mitigasi yang berbeda-beda.\
<br/>

**DORKING LENGKAP <br/>
This is my dorking website for search vulnerability or bug hunting in google, you can use it for sql-injection, xss, pathreversall, and others.<br/><br/>**
*inurl:index.php?id= <br/>
inurl:trainers.php?id= <br/>
inurl:buy.php?category= <br/>
inurl:article.php?ID= <br/>
inurl:play_old.php?id= <br/>
inurl:declaration_more.php?decl_id= <br/>
inurl:Pageid= <br/>
inurl:games.php?id= <br/>
inurl:page.php?file= <br/>
inurl:newsDetail.php?id= <br/>
inurl:gallery.php?id= <br/>
inurl:article.php?id= <br/>
inurl:show.php?id= <br/>
inurl:staff_id= <br/>
inurl:newsitem.php?num= <br/>
inurl:readnews.php?id= <br/>
inurl:top10.php?cat= <br/>
inurl:historialeer.php?num= <br/>
inurl:reagir.php?num= <br/>
inurl:forum_bds.php?num= <br/>
inurl:game.php?id= <br/>
inurl:view_product.php?id= <br/>
inurl:newsone.php?id= <br/>
inurl:sw_comment.php?id= <br/>
inurl:news.php?id= <br/>
inurl:avd_start.php?avd= <br/>
inurl:event.php?id= <br/>
inurl:product-item.php?id= <br/>
inurl:sql.php?id= <br/>
inurl:news_view.php?id= <br/>
inurl:select_biblio.php?id= <br/>
inurl:humor.php?id= <br/>
inurl:aboutbook.php?id= <br/>
inurl:fiche_spectacle.php?id= <br/>
inurl:communique_detail.php?id= <br/>
inurl:sem.php3?id= <br/>
inurl:kategorie.php4?id= <br/>
inurl:news.php?id= <br/>
inurl:index.php?id= <br/>
inurl:faq2.php?id= <br/>
inurl:show_an.php?id= <br/>
inurl:preview.php?id= <br/>
inurl:loadpsb.php?id= <br/>
inurl:opinions.php?id= <br/>
inurl:spr.php?id= <br/>
inurl:pages.php?id= <br/>
inurl:announce.php?id= <br/>
inurl:clanek.php4?id= <br/>
inurl:participant.php?id= <br/>
inurl:download.php?id= <br/>
inurl:main.php?id= <br/>
inurl:review.php?id= <br/>
inurl:chappies.php?id= <br/>
inurl:read.php?id= <br/>
inurl:prod_detail.php?id= <br/>
inurl:viewphoto.php?id= <br/>
inurl:article.php?id= <br/>
inurl:person.php?id= <br/>
inurl:productinfo.php?id= <br/>
inurl:showimg.php?id= <br/>
inurl:view.php?id= <br/>
inurl:website.php?id= <br/>
inurl:hosting_info.php?id= <br/>
inurl:gallery.php?id= <br/>
inurl:rub.php?idr= <br/>
inurl:view_faq.php?id= <br/>
inurl:artikelinfo.php?id= <br/>
inurl:detail.php?ID= <br/>
inurl:index.php?= <br/>
inurl:profile_view.php?id= <br/>
inurl:category.php?id= <br/>
inurl:publications.php?id= <br/>
inurl:fellows.php?id= <br/>
inurl:downloads_info.php?id= <br/>
inurl:prod_info.php?id= <br/>
inurl:shop.php?do=part&id= <br/>
inurl:Productinfo.php?id= <br/>
inurl:collectionitem.php?id= <br/>
inurl:band_info.php?id= <br/>
inurl:product.php?id= <br/>
inurl:releases.php?id= <br/>
inurl:ray.php?id= <br/>
inurl:produit.php?id= <br/>
inurl:pop.php?id= <br/>
inurl:shopping.php?id= <br/>
inurl:productdetail.php?id= <br/>
inurl:post.php?id= <br/>
inurl:viewshowdetail.php?id= <br/>
inurl:clubpage.php?id= <br/>
inurl:memberInfo.php?id= <br/>
inurl:section.php?id= <br/>
inurl:theme.php?id= <br/>
inurl:page.php?id= <br/>
inurl:shredder-categories.php?id= <br/>
inurl:tradeCategory.php?id= <br/>
inurl:product_ranges_view.php?ID= <br/>
inurl:shop_category.php?id= <br/>
inurl:transcript.php?id= <br/>
inurl:channel_id= <br/>
inurl:item_id= <br/>
inurl:newsid= <br/>
inurl:trainers.php?id= <br/>
inurl:news-full.php?id= <br/>
inurl:news_display.php?getid= <br/>
inurl:index2.php?option= <br/>
inurl:readnews.php?id= <br/>
inurl:top10.php?cat= <br/>
inurl:newsone.php?id= <br/>
inurl:event.php?id= <br/>
inurl:product-item.php?id= <br/>
inurl:sql.php?id= <br/>
inurl:aboutbook.php?id= <br/>
inurl:review.php?id= <br/>
inurl:loadpsb.php?id= <br/>
inurl:ages.php?id= <br/>
inurl:material.php?id= <br/>
inurl:clanek.php4?id= <br/>
inurl:announce.php?id= <br/>
inurl:chappies.php?id= <br/>
inurl:read.php?id= <br/>
inurl:viewapp.php?id= <br/>
inurl:viewphoto.php?id= <br/>
inurl:rub.php?idr= <br/>
inurl:galeri_info.php?l= <br/>
inurl:review.php?id= <br/>
inurl:iniziativa.php?in= <br/>
inurl:curriculum.php?id= <br/>
inurl:labels.php?id= <br/>
inurl:story.php?id= <br/>
inurl:look.php?ID= <br/>
inurl:newsone.php?id= <br/>
inurl:aboutbook.php?id= <br/>
inurl:material.php?id= <br/>
inurl:opinions.php?id= <br/>
inurl:announce.php?id= <br/>
inurl:rub.php?idr= <br/>
inurl:galeri_info.php?l= <br/>
inurl:tekst.php?idt= <br/>
inurl:newscat.php?id= <br/>
inurl:newsticker_info.php?idn= <br/>
inurl:rubrika.php?idr= <br/>
inurl:rubp.php?idr= <br/>
inurl:offer.php?idf= <br/>
inurl:art.php?idm= <br/>
inurl:title.php?id= <br/>
trainers.php?id= <br/>
article.php?ID= <br/>
play_old.php?id= <br/>
declaration_more.php?decl_id= <br/>
Pageid= <br/>
games.php?id= <br/>
newsDetail.php?id= <br/>
staff_id= <br/>
historialeer.php?num= <br/>
product-item.php?id= <br/>
news_view.php?id= <br/>
humor.php?id= <br/>
communique_detail.php?id= <br/>
sem.php3?id= <br/>
opinions.php?id= <br/>
spr.php?id= <br/>
pages.php?id= <br/>
chappies.php?id= <br/>
prod_detail.php?id= <br/>
viewphoto.php?id= <br/>
view.php?id= <br/>
website.php?id= <br/>
hosting_info.php?id= <br/>
gery.php?id= <br/>
detail.php?ID= <br/>
publications.php?id= <br/>
Productinfo.php?id= <br/>
releases.php?id= <br/>
ray.php?id= <br/>
produit.php?id= <br/>
pop.php?id= <br/>
shopping.php?id= <br/>
productdetail.php?id= <br/>
post.php?id= <br/>
section.php?id= <br/>
theme.php?id= <br/>
page.php?id= <br/>
shredder-categories.php?id= <br/>
product_ranges_view.php?ID= <br/>
shop_category.php?id= <br/>
channel_id= <br/>
newsid= <br/>
news_display.php?getid= <br/>
ages.php?id= <br/>
clanek.php4?id= <br/>
review.php?id= <br/>
iniziativa.php?in= <br/>
curriculum.php?id= <br/>
labels.php?id= <br/>
look.php?ID= <br/>
galeri_info.php?l= <br/>
tekst.php?idt= <br/>
newscat.php?id= <br/>
newsticker_info.php?idn= <br/>
rubrika.php?idr= <br/>
offer.php?idf= <br/>
"id=" & intext:"Warning: mysql_fetch_array() <br/>
"id=" & intext:"Warning: getimagesize() <br/>
"id=" & intext:"Warning: session_start() <br/>
"id=" & intext:"Warning: mysql_num_rows() <br/>
"id=" & intext:"Warning: mysql_query() <br/>
"id=" & intext:"Warning: array_merge() <br/>
"id=" & intext:"Warning: preg_match() <br/>
"id=" & intext:"Warning: ilesize() <br/>
"id=" & intext:"Warning: filesize() <br/>
index.php?id= <br/>
buy.php?category= <br/>
article.php?ID= <br/>
play_old.php?id= <br/>
newsitem.php?num= <br/>
top10.php?cat= <br/>
historialeer.php?num= <br/>
reagir.php?num= <br/>
intext:"error in your SQL syntax" +site:mm <br/>
intext:"mysql_num_rows()" +site:mm <br/>
intext:"mysql_fetch_array()" +site:mm <br/>
intext:"Error Occurred While Processing Request" +site:mm <br/>
intext:"Server Error in '/' Application" +site:mm <br/>
intext:"Microsoft OLE DB Provider for ODBC Drivers error" +site:mm <br/>
intext:"Invalid Querystring" +site:mm <br/>
intext:"OLE DB Provider for ODBC" +site:mm <br/>
intext:"VBScript Runtime" +site:mm <br/>
intext:"ADODB.Field" +site:mm <br/>
intext:"BOF or EOF" +site:mm <br/>
intext:"ADODB.Command" +site:mm <br/>
intext:"JET Database" +site:mm <br/>
intext:"mysql_fetch_row()" +site:mm <br/>
intext:"Syntax error" +site:mm <br/>
intext:"include()" +site:mm <br/>
intext:"mysql_fetch_assoc()" +site:mm <br/>
intext:"mysql_fetch_object()" +site:mm <br/>
intext:"mysql_numrows()" +site:mm <br/>
intext:"GetArray()" +site:mm <br/>
intext:"FetchRow()" +site:mm <br/>
intext:"Input string was not in a correct format" +site:mm <br/>*
