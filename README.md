# Template

Компактный шаблонизатор.


### Переменная:
Шаблон
```
{PAGE_TITLE}
```
Код
```
$tpl->define_var('PAGE_TITLE', $page_title);
```

### Условие:
Шаблон
```
<!-- IF need_slider -->...<!-- ENDIF -->
```
Код
```
$tpl->define_if('need_slider', true);
```

### Блок:
Шаблон
```
<!-- BLOCK site_main_slider_banners -->
	<div class="swiper-slide">{site_main_slider_banners.CONTENT}</div>
<!-- ENDBLOCK -->
```
Код
```
$tpl->define_block('site_main_slider_banners', [
	'CONTENT' => '...'
]);
```

### Подключение другого шаблона:
Шаблон
```
<!-- INCLUDE calendar.inc.tpl -->
```
