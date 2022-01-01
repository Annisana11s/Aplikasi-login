# Aplikasi-login
Sebuah Aplikasi dengan fitur login
/* Comment: Membuat variabel untuk menyimpan informasi email dan password. */

const loginFormElement = document .querySelector('#loginForm');
const inputEmailElement = document .querySelector('#inputEmail');
const inputPasswordElement = document .querySelector('#inputPassword');

const expectedEmail = 'admin@dicoding.com';
const expectedPassword = 'superpassword';

loginFormElement .addEventListener('submit', fuction(Event) {
   Event. preventDefault();

    /* Comment: Mendapatkan nilai dari masing-masing input (email dan password) ketika tombol ditekan. */ 
   const email = inputEmailElement.value;
   const password = inputPasswordElement.value;

    /* Comment : Memastikan bahwa nilai email dan password sesuai dengan nilai yang tersimpan. */
   if (email == expectedEmail && password == expectedPassword) {

       /* Comment : Jika sesuai maka program akan berpindah ke halaman home */ 
       goToHome();

   } else {
       /* Comment: Namun jika tidak sesuai maka akan menampilkan informasi bahwa input salah. */
       showPopUp();
   }
});
