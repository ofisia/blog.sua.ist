---
title: "1000..."
datePublished: Thu Jan 28 2021 05:00:00 GMT+0000 (Coordinated Universal Time)
cuid: cm89oma9y000n08jvb4sd8xqc
slug: 1000

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1742011020441/66373f74-dbe9-409d-afbb-eb91fd2dd04b.jpeg align="left")

([sumber gambar](https://oldbookillustrations.com/illustrations/title-illustration-1/))

Pagi hari ini saya baru saja menambahkan input sejumlah seribu tautan pada *tumblog* [linklist.ofisia.name](http://linklist.ofisia.name), yang saya bagi dalam empat entri, alias masing-masing berisi dua ratus lima puluh tautan.

Adapun alat-alat bantu dan langkah-langkah yang saya tempuh adalah sebagai berikut, yang sengaja saya catat disini untuk jaga-jaga barangkali saja kelak saya <s>pikun</s> lupa.

* *<s>Cut</s>* potong 250 baris tautan dari total ribuan tautan yang tersimpan dalam Simplenote.
    
* *<s>Paste</s>* tempel pada alat bantu [*regular expression*](https://en.wikipedia.org/wiki/Regular_expression) di situs [**hyperorg**](https://hyperorg.com/misc/ConvertURLsToLinks.html) bikinan bung [David Weinberger](https://weinberger.org), yang akan mengubah baris tautan berformat *plain text* menjadi *tag* HTML.
    
    Contohnya, text [`https://www.example.com/`](https://www.example.com/) akan menjadi `<a href='`[`https://www.example.com/'>https://www.example.com/</a>`](https://www.example.com/'%3Ehttps://www.example.com/%3C/a%3E). [Javascript](https://en.wikipedia.org/wiki/JavaScript) *pancen oye*, terima kasih bung [Brendan Eich](https://en.wikipedia.org/wiki/Brendan_Eich)[.](https://en.wikipedia.org/wiki/BrendanEich)
    
* *<s>Cut and paste</s>* potong dan tempel *tag* HTML pada halaman demo [**Turndown**](https://mixmark-io.github.io/turndown) bikinan bung [Dom Christie](http://domchristie.co.uk).
    
    Turndown akan mengubah contoh `<a href='`[`https://www.example.com/'>https://www.example.com/</a>`](https://www.example.com/'%3Ehttps://www.example.com/%3C/a%3E) menjadi `[`[`https://www.example.com/](https://www.example.com/)`](https://www.example.com/%5D\(https://www.example.com/\)) alias *tag* Markdown.
    
* Potong dan tempel *tag* Markdown pada editor teks apapun—kebetulan saya sedang memakai [Atom](http://atom.io)—lalu <s>lucuti</s> perpendek jumlah karakter URL demi <s>memuaskan selera pribadi</s> estetika.
    
    Sehingga contoh `[`[`https://www.example.com/](https://www.example.com/)`](https://www.example.com/%5D\(https://www.example.com/\)) akan menjadi `[`[`example.com`](http://example.com)`](`[`https://www.example.com/`](https://www.example.com/)`)`.
    
* Masih menggunakan editor teks, tambahkan karakter [*asterisk*](https://en.wikipedia.org/wiki/Asterisk) dan [spasi](https://en.wikipedia.org/wiki/Space_\(punctuation\)) pada awal tiap baris, sehingga contoh `[`[`example.com`](http://example.com)`](`[`https://www.example.com/`](https://www.example.com/)`)` menjadi `* [`[`example.com`](http://example.com)`](`[`https://www.example.com/`](https://www.example.com/)`)`.
    
    *Asterisk* akan menyulap tiap baris Markdown menjadi item-item [*unordered list*](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul). Terima kasih bung [John Gruber](https://en.wikipedia.org/wiki/John_Gruber).
    
* Tetap menggunakan editor teks, bagi jumlah total baris menjadi lima bagian, sehingga masing-masing berjumlah 50 tautan, lalu tambahkan teks `&mdash;` diantaranya.
    
    Teks tersebut bukanlah tag Markdown, namun HTML [*entity*](https://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references#Entities_representing_special_characters_in_XHTML) untuk karakter [*em dash*](https://en.wikipedia.org/wiki/Dash#Em_dash).
    
* Salin dan tempel seluruh baris Markdown diatas ke bidang teks input pada situs [<s>Dillinger</s>](https://dillinger.io) ‹[**Markdown to HTML**](https://markdowntohtml.com),› bikinan bung [Jeremy Thomerson](https://jeremythomerson.com), yang secara ajaib akan mengubah contoh berikut ini ...
    
    ```markdown
    * [example.com](https://www.example.com/)
    * ………
    * ………
    
    &mdash;
    
    * [example.com](https://www.example.com/)
    * ………
    * ………
    ```
    
    … menjadi *tag* HTML berikut ini …
    
    ```xml
    <ul>
    <li><a href="https://www.example.com/">example.com</a></li>
    <li>………</li>
    <li>………</li>
    </ul>
    <p>&mdash;</p>
    <ul>
    <li><a href="https://www.example.com/">example.com</a></li>
    <li>………</li>
    <li>………</li>
    </ul>
    ```
    
* Salin dan tempel output *tag* HTML kembali menuju editor teks, lalu *<s>search and replace</s>* cari dan ganti `</ul>` dengan `</ol>`, serta `<ul>` dengan `<ol start="integer">.`
    
    Dalam hal ini, masing-masing [*integer*](https://en.wiktionary.org/wiki/integer#Noun) adalah `1` , `51` , `101` , `151` , dan `201`, [*respectively*](https://en.wiktionary.org/wiki/respectively#Adverb). Sehingga berakhir menjadi seperti contoh berikut ini ...
    
    ```xml
    <ol start ="1">
    <li>………</li>
    <li>………</li>
    <li>………</li>
    </ol>
    <p>&mdash;</p>
    ………
    ………
    ………
    <p>&mdash;</p>
    <ol start ="201">.
    <li>………</li>
    <li>………</li>
    <li>………</li>
    </ol>
    ```
    
* Ketika sudah berhasil mencapai *<s>boss level</s>* tahap hampir pamungkas ini, saya bisa memberinya predikat tamat bin selesai.
    
    Baris *tag* HTML diatas bisa langsung *cap cus* saya salin tempel ke Tumblr, *publish*, kemudian berangkat tidur dengan nyenyak tanpa *kepikiran*.
    

([sua)](https://sua.ist)