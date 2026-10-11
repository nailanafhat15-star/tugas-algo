# # Tugas-algoritma-Kelompok-11   
**Ainun Naila Nafhat 1251170013 (Project Manager)**   
**Istighfarini 1251170012 (Developer)**     
**Aisyah Nabilah 1251170061 (System Analysis)**  

   BEGIN
  INPUT n = 300            {jumlah dompet dalam tumpukan}  
  INPUT t = 2              {waktu cek per dompet (detik)}  
  INPUT k = 150            {posisi KTM}  

  COMPUTE t_bestcase  = 1   
  COMPUTE t_worstcase = n                   = 300  
  COMPUTE t_average   = (n + 1) / 2        = 150,5   

  FOR i = 1 TO n DO   
    COMPUTE t_selisihbestwaktu = i - t  
    COMPUTE t_vsworstcase      = n / i  
    COMPUTE t_vsaverage        = (n + 1) / (2 * i)  

  OUTPUT "urutan kartu ke", i,   
       "selisih best time :", t_selisihbestwaktu,  
       "percepatan terhadap worstcase :", t_vsworstcase,  
       "percepatan terhadap average :", t_vsaverage  

  OUTPUT "=================================================="  
  OUTPUT judul "ANALISIS PERCEPATAN PENCARIAN KTM (LINEAR SEARCH)"  
  OUTPUT "=================================================="  
  OUTPUT parameter studi kasus:  
    Jumlah dompet dalam tumpukan (N) = 300 kartu  
    Waktu pencarian setiap dompet (t) = 2 detik  
    Posisi KTM yang dicari (k)        = kartu ke-150     
  OUTPUT "=================================================="   
 

  COMPUTE t_bestcase_waktu  = t_bestcase * t       = 2 detik  
  COMPUTE t_worstcase_waktu = t_worstcase * t      = 600 detik   
  COMPUTE t_average_waktu   = t_average * t        = 301 detik  

  OUTPUT "=================================================="     
  OUTPUT " RINGKASAN ANALISIS KASUS "  
  OUTPUT "=================================================="      
  
  OUTPUT hasil ringkasan:   
   Best Case (Kartu ke-1)            : 2.000 s (Langkah 1)    
 - Worst Case (Kartu ke-300)         : 600.000 s (Langkah 300)  
 - Average Case                      : 301.000 s (Langkah 150 )  
 - Selisih Waktu (Worst - Best)      : ( waktu_Worst - waktu_Best)  598.000 s   
 - Percepatan Best terhadap Worst    : ( waktu_worst / waktu_ best ) 300.00x lebih cepat  
 - Percepatan Best terhadap Average  : ( waktu_average / waktu_Best ) 150.50x lebih cepat   
 OUTPUT "=================================================="     
 

    
Selesai  
