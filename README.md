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
