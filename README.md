// problem: Mengapa perlu ada optional ?

//rules :
//1. setiap variabel harus didefinisikan secara (implicit/explicit)
//2. tipe/jenis variable dapat ditentukan berdasarkan valuenya
//3. setiap tipe normal harus memiliki nilai yang terkait

//implicit and explicit

let name: String = "fadielse"  //explicit
let newName = "fadielse the developer" //implicit

let myAge: Int = 20  //explicit
let myBrotherAge = 14 //implicit
let myGPA: Double = 3.54 //explicit


//Jika kita ingin mengembalikan dengan suatu nilai atau nil
let myFaceOne = "Handsome"
//let myFaceTwo = nil
//jadi untuk menangani ini (nil value) kita menggunakan optional "?"
//tipe optional memungkinkan menyimpan nil
let myName: String? = nil
let yourName: String? = "Fadielse"

print(yourName)
//jadi berdasarkan kode sebelumnya menghasilkan 
//optional rules :
//1. opsional tidak saling berinteraksi
//2. convert optional ke tipe normal, proses ini dikenal dengan unwrapping

//1.Forced unwrapping
print(yourName!)

//MASALAH yang sering terjadi ketika menggunakan Force Unwrapping
//var image: String? = nil
//let normalImage = image!
//2 baris kode diatas jika dijalankan akan menyebabkan aplikasi mengalami CRASH

//Gunakan
//2. implicit unwrapping
let imageFromInstagram: String? = "Fadielse's Face"

if let normalImage = imageFromInstagram {
    print(normalImage)
} else {
    print("tidak ada gambar")
}
