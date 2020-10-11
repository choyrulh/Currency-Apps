# Currency Apps
Aplikasi ini mencakup fungsi perhitungan nilai tukar nilai mata uang rupiah dari dollar. Satu dollar dianggap Rp 15.000,00

## Scope & Functionalities
- User dapat memasukkan angka
- User dapat mengeklik tombol hitung
- User mendapat info invalid jika memasukkan berupa teks/huruf

## How does it works
Diawali dari method "MainWindow" pada class window.xaml.cs dideklarasikan dengan:

``` csharp
public MainWindow()
        {
            InitializeComponent();
            Currency = new CurrencyController();
        }
```
logika perhitungan terdapat pada CurrencyController.cs sebagai berikut:
``` csharp
public string usdToIdr(string nominal)
        {
            var nominalDouble = Convert.ToDouble(nominal);
            var result = nominalDouble * 15000;
            return Convert.ToString(result);
        }
```



