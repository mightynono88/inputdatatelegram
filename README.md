# inputdatatelegram
var token = "no kode"; // ambil token dari bot Father telegram
var ssId = "no kode"; // ambil ID pada URL database spreadsheets
var WebAppUrl = "url"; // ambil url hasil publish

var telegramUrl = "https://api.telegram.org/bot" + token;

//cukup Jalankan/Run Fungsi setWebhook sekali
function setWebhook() {
var url = telegramUrl + "/setWebhook?url=" + WebAppUrl;
var response = UrlFetchApp.fetch(url);
}

//persiapan pengiriman data
function sendText(id,text) {
  var url = telegramUrl + "/sendMessage?chat_id=" + id + "&text=" + encodeURIComponent(text);
  var response = UrlFetchApp.fetch(url);
  Logger.log(response.getContentText());
}menocba lagi
ada
