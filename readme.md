Deskripsi       : Membuat tugas Gradle untuk menerima pesan ucapan sederhana dan di push ke Github
Langkah-langkah : - menggunakan software intelliJ IDEA create new project gradle
                  - adding dependencies di build.gradle implementation 'com.google.guava:guava:29.0-jre' testImplementation 'junit:junit:4.13'}
                  - adding task greatingTask(){
                                doLast {
                                String nama = project.hasProperty('nama') ? project.property('nama') : 'Riana'
                                println "Hello, $nama! Welcome to Gradle World!"
                                        }
                                }
                  - di terminal menjalankan git init
                                            git remote -v
                                            git add .
                                            git commit -m "first commit"
                                            git branch -M main
                                            git remote add origin https://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@github.com/rianardiansari/learnGradletask.git
                                            git add .
                                            git commit -m "adding readme.md"
                                            git push -u origin main
                                            ./gradlew greatingTask -Pnama=eko
Tujuan       : untuk menerima pesan ucapan "Hello, eko! Welcome to Gradle World" 
<img width="750" alt="Screenshot 2023-11-22 at 08 30 31" src="https://github.com/rianardiansari/learnGradletask/assets/149749846/08307015-0a8c-422a-b6c9-ee0d77160996">
