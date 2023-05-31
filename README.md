# CVИванкевич Вадим

Дата рождения: 02.09.2004
Проживание: г. Витебск, ул. Марка 48

Готов к переезду в г. Минск
Контактная информация: Телефон: +375 (29) 234 45 65 Электронная почта: a.Vadim@mail.ru

Желаемая должность: Экономист-программист

Желаемый уровень дохода: 2000 рублей

Ключевые навыки: Знание языка с++, хорошее владение exel и word

Достижения: Создал компьютерную программу с «0». Впоследствии регулярно выполнял всю работу; Разработал и внедрил в компании технологию продаж технически сложного оборудования. Опыт работы: Отсутствует Сфера деятельности компании: разработка ПО Расширение клиентской базы; Работа с ключевыми клиентами, устранение возникших разногласий; Своевременный и систематический мониторинг цен аналогичной продукции конкурентов. Образование: 2025 ВГУ Машерова. Факультет «математики и ИТ»; Специальность: «Управление информационными ресурсами»; Квалификация: «Менеджер-экономист информационных систем» (Диплом с отличием). 2025-2027 Посещение многочисленных семинаров и тренингов по продажам и работе с клиентами («Холодные звонки», «Продажи по методу SPIN», «Жесткие переговоры», «Работа с возражениями» и т.д.) Дополнительная информация: Иностранные языки: английский язык – advanced. Знание ПК: уверенный пользователь (MS Office; CRM; 1С;c++;JAVA SCRIPT). Пример кода:
function lib() { var _windowContainer = null, _guid = null, _poll = this, _name = '', _store = null; var header, panel; var save = function(){ //Функция сохранения изменений в анкете if (!panel.container['form'].pharmId) return false; var modifyData = ''; $.each(_store.getModifiedRecords(), function(index, rec){ $.each(rec.modified, function(name){ modifyData += '&values['+index+']['+name+']=' + rec.data[name]; }); modifyData += '&id['+index+']=' + rec.id; }); if (modifyData == '') return; $.getJSON('./modules/units/units.php?action=SET_FORMDATA&pharmId='+panel.container['form'].pharmId+'&projectId='+_param.projectId+'&stageId='+_param.stageId + modifyData +'&rnd='+Math.random(), function(data){ if (!data || !data.result){ alert('ошибка сохранения, попробуйте еще раз'); //_store.rejectChanges(); }else if (data.result == true){ _store.commitChanges(); panel.container['form'].loadData(panel.container['form'].pharmId); } $.unblockUI(); }.bind(this)); } var Header = function (container) { var id = 'li[rel = "' + _guid + '"] '+ ".context"; var template = '

 
'; Header.superClass.apply(this, [id, template, container]); this.appendTo = function (parent) { $(parent).append(this.template); return this; } var _expanded = true; this.expand = function(callback){ _expanded = true; _windowContainer.find('.header_button').removeClass('expand').addClass('collapse'); this.element().animate({ height: this.container['title'].element().outerHeight() + this.container['description'].element().outerHeight() }, "fast", callback); } this.height = function (height) { return _windowContainer.find('.header').outerHeight() } this.expanded = function(){ return _expanded; } this.addButton = function(caption, delegate){ _windowContainer.find('.buttons').append(''); _windowContainer.find('.buttons #'+caption).click(delegate); } this.collapse = function(callback){ _expanded = false; _windowContainer.find('.header_button').removeClass('collapse').addClass('expand'); this.element().animate({ height: this.container['title'].element().outerHeight() }, "fast", callback); } this.toggle = function(callback){ if (_expanded){ this.collapse(callback); }else{ this.expand(callback); } } this.click = function(delegate){ if (!delegate){ _windowContainer.find('.header_button').click(); }else{ _windowContainer.find('.header_button').unbind().click(delegate); } } } Header.inherits(App.VisualElement);//Наследуем элемент от базового из файла part_of_core.js var Title = function(){ var id = 'li[rel = "' + _guid + '"] '+ ".title"; var template = '
Приближая весну
'; Title.superClass.apply(this, [id, template]); } Title.inherits(App.VisualElement); var Description = function(){ var id = 'li[rel = "' + _guid + '"] '+ ".description"; var template = '
'; Description.superClass.apply(this, [id, template]); } Description.inherits(App.VisualElement); var Panel = function(container){ var id = 'li[rel = "' + _guid + '"] '+ ".panel"; var template = '
'; Panel.superClass.apply(this, [id, template, container]); } Panel.inherits(App.VisualElement); var Grid = function () { var id = 'li[rel = "' + _guid + '"] '+ ".grid"; var template = ''; Grid.superClass.apply(this, [id, template]); var store = new Ext.data.JsonStore({// аналог "DataTable" из состава ExtJS root: 'units', totalProperty: 'count',
