# Currency Apps
Aplikasi yang mencakup perhitungan nilai mata uang dari dollar ke
rupiah. Satu dollar senilai Rp.14.000

## Scope & Functionalities
- User dapat memasukkan angka
- User dapat mengeklik tombol hitung
- User mendapat info "INVALID" jika yang dimasukkan text
 
## How Does it works?
Diawali dari method Mainwindow pada class Mainwindow.xaml.cs, dan 
dilanjutkan dengan mendeklarasikan class CurrencyController

    public MainWindow()
        {
            InitializeComponent();
            currency = new CurrencyController();
        }

dan logika perhitungannya terdapat pada class CurrencyController.cs sebagai berikut.


    public string usdToIdr(string nominal)
        {
            var nominalDouble = Convert.ToDouble(nominal);
            var result = nominalDouble * 15000;
            return Convert.ToString(result);
        }
cara kerjanya ialah pada saat memasukkan sebuah nominal berapapun itu dikali dengan
15000