# Bitirme Projesi

## Proje Hakkında

[Proje Detayları](/files/e-cozum-bitirme.pdf)

[Sena'ya mail ile yollamanız gereken dosya](/files/Bitirme-Projesi-Hazirlik-Dokumani.docx)

## Api çalıştırma

1.  Api reposunu klonla

    `git clone https://github.com/haandev/patika-kanban-api.git`

2.  Proje dizinine gir

    bash: `cd patika-kanban-api/`

    powershell: `cd .\bitirme-projesi\`

3.  Docker buildini al

    `docker-compose build`

4.  Ayağıya kaldırma

    `docker-compose up`

## Postman

1. [Bu](/files/Kanban-Board-App.postman_collection.json) dosyayı indir

2. Json dosyasını postmana aktarma

   ![gif](/files/postman.gif)

**Not-1**

> Repo güncellendiğinde git pull dedikten sonra 3. aşamadan itibaren işlemleri tekrardan yapın

**Not-2**

> İlk çalıştırmada hata alabilirsiniz, kapatıp tekrar `docker-compose up` komutunu deneyin

**İşinize yarayabilecek bazı repolar**

- [axseinga/kanbanboard-app-react](https://github.com/axseinga/kanbanboard-app-react?ref=reactjsexample.com)
- [asseinfo/react-kanban](https://github.com/asseinfo/react-kanban)
- [szymonsuchanowski/kanban-app](https://github.com/szymonsuchanowski/kanban-app)
