package main

import "fmt"

// =====================
// SOAL 1
// =====================
func cekDigit() {
	var x, n int
	var ulang string

	for { // LOOPING SOAL 1
		fmt.Print("Masukkan nilai x: ")
		fmt.Scan(&x)

		fmt.Print("Masukkan nilai n: ")
		fmt.Scan(&n)

		ditemukan := false

		for n > 0 { // LOOPING CEK DIGIT
			if n%10 == x {
				ditemukan = true
			}
			n = n / 10
		}

		fmt.Println("Hasil:", ditemukan)

		fmt.Print("Ulang soal 1? (y/n): ")
		fmt.Scan(&ulang)
		if ulang != "y" {
			break
		}
	}
}

// =====================
// SOAL 2
// =====================
func daunTerlebar() {
	var n int
	fmt.Print("Masukkan jumlah daun: ")
	fmt.Scan(&n)

	var max, lebar int

	for i := 1; i <= n; i++ { // LOOP INPUT DAUN
		fmt.Printf("Masukkan lebar daun ke-%d: ", i)
		fmt.Scan(&lebar)

		if i == 1 || lebar > max {
			max = lebar
		}
	}

	fmt.Println("Daun paling lebar:", max)
}

// =====================
// SOAL 3
// =====================
func digitTerbesar() {
	var n int
	var ulang string

	for { // LOOPING SOAL 3
		fmt.Print("Masukkan bilangan: ")
		fmt.Scan(&n)

		max := 0

		for n > 0 { // LOOP CEK DIGIT
			digit := n % 10
			if digit > max {
				max = digit
			}
			n = n / 10
		}

		fmt.Println("Digit terbesar:", max)

		fmt.Print("Ulang soal 3? (y/n): ")
		fmt.Scan(&ulang)
		if ulang != "y" {
			break
		}
	}
}

// =====================
// MAIN
// =====================
func main() {

	var pilihan int

	for { // LOOPING MENU UTAMA
		fmt.Println("\n===== MENU =====")
		fmt.Println("1. Cek digit")
		fmt.Println("2. Daun terlebar")
		fmt.Println("3. Digit terbesar")
		fmt.Println("0. Keluar")
		fmt.Print("Pilih: ")
		fmt.Scan(&pilihan)

		switch pilihan {
		case 1:
			cekDigit()
		case 2:
			daunTerlebar()
		case 3:
			digitTerbesar()
		case 0:
			fmt.Println("Program selesai")
			return
		default:
			fmt.Println("Pilihan salah!")
		}
	}
}
