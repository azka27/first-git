# first-git
First using git

git --version  						  -> mengetahui versi berapa
git config --global user.name "Azka"                      -> Konfigurasi nama
git config --global user.email azka27wicaksana@gmail.com  -> konfigurasi email
git config --list 					  -> Memeriksa list konfigurasi
git init nama_proect 					  -> Membuat repository/ membuat direktori proyek
git status						  -> Melihat status repository
git add nama_file					  -> Mengubah file modified menjadi staged
contoh lain: git add nama_file1 nama_file2 nama_file3
	     git add *.html
	     git add					  -> Semua file dan direktor
git commit						  -> Mengubah file dari staged menjadi commited
git commit -m "Revisi berubah"				  -> Menambahkan pesan pada perubahan
git log							  -> Melihat catatan log perubahan pada direktori
contoh lain: git log --oneline				  -> Menampilkan log yg lebih pendek
	     git log f5ab02679fdf34a152d535528e7b2aabb4	  -> Dengan nomor revisi
	     git log nama_file.html			  -> Melihat pada file tertentu
git log --author='nama_author'				  -> Melihat revisi apa saja pada org tertentu
git diff 227f93bf5ca3369fadf48dbca4e310b8376a7ab7	  -> Melihat perubahan yg dilakukan pada revisi
contoh lain: git diff index.html			  -> Melihat perbandingan pada file 
git checkout nama_file.html				  -> Membatalkan revisi sebelum staged dan commited (temporer)
git reset nama_file.html				  -> Membatalkan revisi sesudah staged sebelum commited
git reset --soft <nomor_commit>				  -> Membatalkan revisi (tdk temporer) dalam kondisi staged
git reset --mixed <nomor_commit>			  -> Membatalkan revisi (tdk temporer) dalam kondisi modified
git reset --hard <nomor_commit>				  -> Membatalkan revisi (tdk temporer) dalam kondisi commited
git checkout c5c9dfe4c18674bf1533c9b237667 nama_file.html -> Membatalkan revisi sesudah staged dan commited
contoh lain: git checkout c5c9dfe4c18674bf1533c9b237667   -> Membatalkan revisi sesudah staged dan commited (seluruh file)
git checkout HEAD~3 index.html				  -> Membatalkan revisi kembali ke 3 commied sebelumnya (temporer)
git revert -n <nomor_commit>				  -> Membatalkan revisi seluruh file ke suatu commited (temporer)
git branch nama_cabang					  -> Membuat cabang di repository
git branch						  -> Melihat daftar branch
git checkout nama_cabang				  -> Berpindah ke cabang yang ingin ditindak
git merge nama_cabang					  -> Menggabungkan cabang ke master
git branch -d nama_cabang				  -> Menghapus nama cabang yang tidak perlu
