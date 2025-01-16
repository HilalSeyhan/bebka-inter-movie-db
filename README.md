https://drive.google.com/file/d/1d3NywGuqiPjpO7SeR4fp00F3gNlvFobg/view?usp=drive_link

## Başlarken

- Bu depoyu klonlayın (ssh bağlantınızın düzgün bir şekilde kurulduğundan emin olun) - Kod düzenleyicinizde [prettier](https://prettier.io/) yüklü olduğundan emin olun - Ayrıca tarayıcınızda [pesticide browser extension](https://chrome.google.com/webstore/detail/pesticide-for-chrome-with/neonnmencpneifkhlmhmfhfiklgjmloi) yüklü olduğundan emin olun.

---

## Adlandırma Kuralları ve En İyi Uygulamalar

Bu proje üzerinde çalışırken uygun adlandırma kurallarına ve en iyi uygulamalara uymak önemlidir. Bu, temiz ve okunabilir bir kod tabanını korumamıza yardımcı olacaktır. Bu aynı zamanda birleştirme çakışmalarından ve yanlış adlandırma kurallarından kaynaklanabilecek diğer sorunlardan kaçınmamıza yardımcı olur.

### Adlandırma Kuralları ve Bir Bilet Nasıl Tamamlanır

Bir bilet üzerinde çalışırken, öncelikle `master` dalındaki en son değişikliklere sahip olduğunuzdan emin olmanız gerekir. Bunu yapmak için aşağıdaki komutları çalıştırın:

``bash git checkout master

git pull origin master ```

En son değişiklikleri `master` dalından çektikten sonra, artık biletiniz üzerinde çalışmak için yeni bir dal oluşturabilirsiniz. Yeni bir dal oluşturmak için aşağıdaki komutu çalıştırın:

`bash git checkout -b <branch-name> `

<branch-name>` aşağıdaki formatta olmalıdır:

`bash <adınız>/<bilet-numarası>-<bilet-başlığı-veya-açıklama> `

Örneğin, `CO-120` numaralı bilet üzerinde çalışıyorsanız ve adınız `John Doe` ise, şube adınız şöyle olmalıdır:

``bash johnDoe/CO-120-hero-section ```

Şubenizi oluşturduktan sonra, artık biletiniz üzerinde çalışmaya başlayabilirsiniz. Biletiniz üzerinde çalışmayı bitirdiğinizde, artık değişikliklerinizi uzak depoya gönderebilirsiniz. Bunu yapmak için aşağıdaki komutları çalıştırın:

``bash git add .

git commit -m "[<ticket-number>] - <commit-message>" ```

Örneğin, `CO-120` bileti üzerinde çalışıyorsanız ve kahraman bölümü için HTML işaretlemesini uyguladıysanız, commit mesajınız şöyle olmalıdır:

``bash git commit -m "[CO-120] - Implemented HTML markup" ```

Değişikliklerinizi işledikten sonra, artık değişikliklerinizi uzak depoya gönderebilirsiniz. Bunu yapmak için aşağıdaki komutu çalıştırın:

``bash git push origin <branch-name> ```

Örneğin, `CO-120` bileti üzerinde çalışıyorsanız ve dalınızın adı `johnDoe/CO-120-hero-section` ise, aşağıdaki komutu çalıştırmalısınız:

``bash git push origin johnDoe/CO-120-hero-section ```

Değişikliklerinizi uzak depoya gönderdikten sonra, artık bir çekme isteği oluşturabilirsiniz. Bunu yapmak için [repository](https://github.com/archis-academy/July-Bebka-Beginner-Grover-2) adresine gidin ve `Pull requests` sekmesine tıklayın. Ardından `Yeni çekme isteği` düğmesine tıklayın. Temel dalın `master` ve `karşılaştırma` dalının `<şube-adı>` olduğundan emin olun. Çekme isteğinin başlığının biçimi şöyle olmalıdır:

`bash [<ticket-number>] - <ticket-title-or-description> `

Örneğin, `CO-120` bileti üzerinde çalışıyorsanız ve kahraman bölümü için HTML işaretlemesini uyguladıysanız, çekme isteğinizin başlığı şöyle olmalıdır:

``bash [CO-120] - Kahraman bölümü için HTML işaretlemesi ```

Kendinizi atadığınızdan ve ekip arkadaşlarınızı ve ekip liderinizi gözden geçiren olarak eklediğinizden emin olun. Bundan sonra, `Çekme isteği oluştur` düğmesine tıklayın ve `Lokum` üzerindeki bileti çekme isteğinin bağlantısıyla güncelleyin.

![Assign the ticket to yourself](https://33333.cdn.cke-cs.com/kSW7V9NHUXugvhoQeFaf/images/3246ff0603e48fe80d5a0345d47141f50bae23e8fc3b9e52.png/w_336)

![Assign reveiwers to the ticket](https://user-images.githubusercontent.com/71005514/284887977-9bece5e1-ee6b-4ffb-b098-d093ee31a52d.png)

### En İyi Uygulamalar

- Bir commit göndermeden önce tüm görevin tamamlanmasını beklemeyin. Görevinizi daha küçük parçalara ayırın ve bir parça tamamlandığında bir commit gönderin.

---
