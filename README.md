ДЕМО САЙТ https://bahek2462774.github.io/jquery.EmbedVkGallery/


Описание
=
Плагин добавляет фотографии из альбомов "ВК" а так же выравнивает их в равномерную по ширине плитку (IE9+)

Важно! Альбом должен быть открыт для просмотра любым пользователем. 

Параметры можно передать в data атрибутах, либо объектом. Так же можно передать только ссылку на альбом.

параметры
=
full_image_size = Размер картинки, которая будет открыватся по клику (по умолчанию = 'x')
Если скрипт не находит нужную картинку - попытается взять сначала 'm', потом 's'.
Если ничего не найдено - пропустит эту картинку.
Все описания форматов есть в доке к VK API https://vk.com/dev/photo_sizes

shuffle (по умолчанию 0) - перемешивает массив с фотографиями

width - приблизительная ширина плитки. ( 100 по умолчанию )

margin - отступы между плитками. (4 по умолчанию )

limit - лимит картинок - которые будут загружены и показаны. 

rev - по умолчанию 1 ( выводит фотографии в антихронологичном порядке добавления )

link - ссылка на альбом. 

пример
=
$(‘#vk’).EmbedVkGallery();

$('#vk2).EmbedVkGallery('http://vk.com/album-27725748_154688860');

 $('#vk3').eq(2).EmbedVkGallery({
                link: 'http://vk.com/album-27725748_138005450',
                margin: 5
            });


Просмотр картинок осуществляет плагин slibmox2 http://www.digitalia.be/software/slimbox2