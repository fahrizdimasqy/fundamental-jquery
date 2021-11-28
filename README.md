# fundamental-jquery
### Seleksi Element
```javascript
// seleksi element
$("button"); //berfungsi seperti querySelector dan querySelectorAll
```

### Manipulasi Stylesheet
```javascript
// manipulasi stylesheet
$("h1").css("color", "red");
// parameter pertama properti mana yang diubah
// parameter kedua adalah nilai yang diubah

// jika hanya 1 pamarameter kita hanya akan mendapatkan nilainya saja
// jika 2 paramter maka kita mengubah nilainya
```

### Menambahkan dan menghapus kelas css ke element
```javascript
// menambah class css ke element
$("h1").addClass("big-title");

// menghapus class menggunakan removeClass
$("h1").removeClass("big-title");
// mengecek ada atau tidaknya class menggunakan hasClass
$("h1").hasClass("big-title");
```
### Memanipulasi text
```javascript
// manipulasi text
$("h1").text("Hello Fahriz");
// sama seperti innerText

$("h1").html("<em> Fahriz </em>");
// sama seperti innerHtml
```

### Memanipulasi attribute element

```javascript
// manipulasi attributes
$("img").attr("src", "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/1200px-React-icon.svg.png");

$("a").attr("href", "https://bing.com");
```
### Menggunakan Event Listener Di jQuery

```javascript
// add event listener
$(document).keypress(function(event) {
  $("h1").html(event.key);
});
```

### Menambah dan menghapus element

```javascript
// menambahkan element
$("h1").before("<button> New </button>");
// akan ditambahkan sebelum tag pembuka element yang dipilih

$("h1").after("<button> New </button>");
// akan ditambahkan sesudah tag pembuka element yang dipilih

$("h1").prepend("<button> New </button>");
// menambahkan element tepat sebelum konten element yang dipilih dan tepat tag pembuka
// <h1><button>New</button>Helllo</h1>

$("h1").append("<button> New </button>");
// <h1>Hello<button>New</button></h1>
// menambahkan element tepat setelah konten element yang dipilih dan tepat tag pembuka

// mengapus element
$("button").remove();
```
### Animasi 
```javascriot
// animation
$("button").on('click', function() {
  $("h1").toggle();
});
```

```javascript
$('h1').on('click', function() {
  $("h1").fadeToggle();
});
```
```javascript
$('h1').on('click', function() {
  $("h1").animate({
    opacity: 0.5
  });
});
```
