# TimoninArtBot
 import telebot
from telebot import types
from random import *
import time
import random

bot = telebot.TeleBot('5326365875:AAHWqYLAMrwPnVPkI_rG133UPgEs2LpegYM')

@bot.message_handler(commands=['s1'])
def s1(message):
    markup = types.InlineKeyboardMarkup(row_width=1)
    r1=['Как сосиска в тесте, тепло и тесно.','Дела мои амбивалентно…',
        'Еще никого не убил, но уже близок к этому.','Бьет ключом, да всё по голове.',
        'В порядке, только вот в случайном.']
    item1 = types.InlineKeyboardButton(choice(r1), callback_data='z1')
    r2 = ['В шоколаде все, клавиатура в том числе.', 'Вроде бы все отлично, только вот никто не завидует.',
          'Все в ажуре, когда сидишь на абажуре…', 'Все дела переданы прокурору.', 'Все пучком — нос торчком!']
    item2 = types.InlineKeyboardButton(choice(r2), callback_data='z2')
    r3 = ['Как в сценарии — развязка близко.', 'Два дня на карете, неделю пешком.',
          'Дела бывают у того, кто что-то делает, а я – отдыхаю!', 'Дела идут хорошо, когда выпьешь да ишшо.',
          'Дела как в аптеке – все дорого, но нужно.']
    item3 = types.InlineKeyboardButton(choice(r3), callback_data='z3')
    r4 = ['Не буду отвечать!', 'Не хочу отвечать!', 'Мне лень отвечать!', 'Я забыл что отвечать!',
          'Я не уверен как отвечать']
    item4 = types.InlineKeyboardButton(choice(r4), callback_data='z4')
    markup.add(item1, item2, item3, item4)
    bot.send_message(message.chat.id, 'Вопрос: 1-7\nНу что свободный Художник, давай оценивать твою будущую мазню! '
                                      'Чем дышишь, ''как твои дела? Не мандражируй, выбери близкую по духу '
                                      'строчку!', reply_markup=markup)


@bot.message_handler(commands=['s2'])
def s2(message):
    markup = types.InlineKeyboardMarkup(row_width=1)
    r5=['Сюрреализм это чудо чудесное','Сюрреализм размягчает сознание!','Сюрреализм удел лидеров!',
        'Сюрреализм форточка в свободу!','Сюрреализм - стиль жизни']
    item5 = types.InlineKeyboardButton(choice(r5), callback_data='z5')
    r6 = ['Сюрреализм - это глоток воздуха!', 'Сюрреализм - это пропус в рай!', 'Сюрреализм - это манна небесная!',
          'Сюрреализм - это шаг в матрицу!', 'Сюрреализм - это ширма гениальности!']
    item6 = types.InlineKeyboardButton(choice(r6), callback_data='z6')
    r7 = ['Сюрреализм - это луч в непознанное!', 'Сюрреализм - это воплощенный креатив!',
          'Сюрреализм - это искусство пришельцев!', 'Сюрреализм - это танец сознания!',
          'Сюрреализм - это искусство избранных!']
    item7 = types.InlineKeyboardButton(choice(r7), callback_data='z7')
    r8 = ['Мне лень гуглить!', 'Я не отдупляю!', 'Я стараюсь не думать!', 'Я боюсь думать об этом!', 'Кто здесь?']
    item8 = types.InlineKeyboardButton(choice(r8), callback_data='z8')
    markup.add(item5, item6, item7, item8)
    bot.send_message(message.chat.id, 'Вопрос: 2-7\nЧто для тебя Сюрреализм? Собери волю в кулак, утри сопли, постарайся подумать...'
                                      'Хоть немного подумать! Чуть-чуть!', reply_markup=markup)


@bot.message_handler(commands=['s3'])
def s3(message):
    markup = types.InlineKeyboardMarkup(row_width=1)
    r9 = ['Разведу блинную муку!', 'Буду разбрызгивать Квас!', 'Натолку листья подорожника!',
          'Стырю в метро огнетушитель!', 'Налью воды из фонтана на ВДНХ!']
    item9 = types.InlineKeyboardButton(choice(r9), callback_data='z9')
    r10 = ['Попрошу краску у соседа!', 'Буду клянчить в Леруа Мерлен!', 'Смешаю все из холодильника!',
           'Буду размазывать грязь из лужи!', 'Деньги есть - буду шампанским!']
    item10 = types.InlineKeyboardButton(choice(r10), callback_data='z10')
    r11 = ['Расплавлю целофановые пакеты!', 'Куплю жидкость в аптеке', 'Найду сосуд в пустыне',
           'Буду плеваться и рыгать!', 'Что под руку попадется!']
    item11 = types.InlineKeyboardButton(choice(r11), callback_data='z11')
    r12 = ['Закажу в Яндекс Доставке!', 'Закажу  на Ozon!', 'В слепую куплю на ebay!',
           'выберу в Wildberries', 'спрошу у Джигурды!']
    item12 = types.InlineKeyboardButton(choice(r12), callback_data='z12')
    markup.add(item9, item10, item11, item12)
    bot.send_message(message.chat.id, 'Вопрос: 3-7\nЧем планируешь создавать эффект? т.е. чем собираешься мазюкать? '
                                      'т.е. краска у тебя хоть есть? ', reply_markup=markup)


@bot.message_handler(commands=['s4'])
def s4(message):
    markup = types.InlineKeyboardMarkup(row_width=1)
    r13 = ['На стене в поликлинике!', 'На коробке от сандаликов!', 'На снеговике!', 'На подошве утюга!',
           'На дне вулкана!']
    item13 = types.InlineKeyboardButton(choice(r13), callback_data='z13')
    r14 = ['На линолеуме в магазине!', 'Куплю типа холст!', 'На туалетной бумаге!', 'На глади морской!',
           'На двери УАЗика соседа!']
    item14 = types.InlineKeyboardButton(choice(r14), callback_data='z14')
    r15 = ['На спине укуренного растамана!', 'На стейке говядины!', 'На яичке курином!',
           'На ракете С300 после взлета!', 'На костюме в примерочной!']
    item15 = types.InlineKeyboardButton(choice(r15), callback_data='z15')
    r16 = ['Я не решил!', 'Я не могу сообразить', 'Я далек от поверхностей!', 'А что, это надо знать?',
           'Я жду сон - мне приснится!']
    item16 = types.InlineKeyboardButton(choice(r16), callback_data='z16')
    markup.add(item13, item14, item15, item16)
    bot.send_message(message.chat.id, 'Вопрос: 4-7\nНа чем будешь искусство проявлять? Поверхность какая? Не '
                                      'выпендривайся, выбирай из предложенного!', reply_markup=markup)


@bot.message_handler(commands=['s5'])
def s5(message):
    markup = types.InlineKeyboardMarkup(row_width=1)
    r17 = ['Я бессмертный, время пофиг!', 'От среды до столба!', 'Я заведу часы с кукушкой!', 'Время? Я не смотрю ТВ!',
           'Сменю часовой пояс!']
    item17 = types.InlineKeyboardButton(choice(r17), callback_data='z17')
    r18 = ['Время лечит, я бухну!', 'Время не воробей, оно не клюет!', 'Временные факторы в игнор!',
           'Не время говорить - Время!', 'Время может пойти вспять!']
    item18 = types.InlineKeyboardButton(choice(r18), callback_data='z18')
    r19 = ['Машину времени к подъезду!', 'Я постараюсь выжить к окончанию!', 'Попробую измерить курвиметром!',
           'Летаргический сон - наше все!', 'Пустим ка время - на самотек!']
    item19 = types.InlineKeyboardButton(choice(r19), callback_data='z19')
    r20 = ['Я ношу часы на руке!', 'Я слежу за временем!', 'Я пунктуален!', 'Я никогда не опаздываю!',
           'Я ценю свое время!']
    item20 = types.InlineKeyboardButton(choice(r20), callback_data='z20')
    markup.add(item17, item18, item19, item20)
    bot.send_message(message.chat.id, 'Вопрос: 5-7\nКак долго планируешь заниматься этой фигней? Сколько времени готов '
                                      'потратить на креатив?', reply_markup=markup)


@bot.message_handler(commands=['s6'])
def s6(message):
    markup = types.InlineKeyboardMarkup(row_width=1)
    r21 = ['Горизонта не существует!', 'Мухи тоже вертолет!', 'Ослик любит шарики!', 'Давление живет в барометре!',
           'Мысли можно на масло намазать!']
    item21 = types.InlineKeyboardButton(choice(r21), callback_data='z21')
    r22 = ['Саженцы попробую в небо воткнуть!', 'Бамбук сложно раскуривать!', 'Я не габбер, я сидун!',
           'Стрелка не направление!', 'Кодовый замок придумали терпилы!']
    item22 = types.InlineKeyboardButton(choice(r22), callback_data='z22')
    r23 = ['Игра змейка - как ремень для трусов!', 'Опилки алюминия - не для солонки!',
           'Космос сегодня отзеркаливает видениями!', 'Квадрат Малевича - не квадрат!', 'Я бархат, положу на мох!']
    item23 = types.InlineKeyboardButton(choice(r23), callback_data='z23')
    r24 = ['Что бы маме понравилось!', 'Что бы коллеги не засмеяли!', 'Что бы грамоту получить!',
           'Что бы Джигурда руку пожал!', 'Не хочу проблемы!']
    item24 = types.InlineKeyboardButton(choice(r24), callback_data='z24')
    markup.add(item21, item22, item23, item24)
    bot.send_message(message.chat.id, 'Вопрос: 6-7\nЧто в первую очередь планируешь учесть при создании '
                                      'произведения искусства?', reply_markup=markup)


@bot.message_handler(commands=['s7'])
def s7(message):
    markup = types.InlineKeyboardMarkup(row_width=1)
    r25 = ['Планирую купить поесть!', 'Хочу попробовать съесть кг черной икры!', 'Мне нужен хлеб!',
           'Мне надо набрать вес!', 'Буду открывать фабрику, делать торты!']
    item25 = types.InlineKeyboardButton(choice(r25), callback_data='z25')
    r26 = ['Хочу помочь Спайдермену!', 'Планирую конкурировать с Шреком!', 'Хочу стать габбером!',
           'Желаю снести Москва Сити!', 'Хочу удивить Джигурду!']
    item26 = types.InlineKeyboardButton(choice(r26), callback_data='z26')
    r27 = ['Буду строить континент!', 'Буду углублять океаны!', 'Хочу в космос,начили!', 'Хочу мир перевернуть!',
           'Хочу мировую Арт революцию затеять!']
    item27 = types.InlineKeyboardButton(choice(r27), callback_data='z27')
    r28 = ['Я за мир во всем мире!', 'Просто хочу быть знаменитым!', 'Хочу быть признанным художником!',
           'Хочу всесторонне развиться!', 'Хочу просто стать успешным!']
    item28 = types.InlineKeyboardButton(choice(r28), callback_data='z28')
    markup.add(item25, item26, item27, item28)
    bot.send_message(message.chat.id, 'Вопрос: 7-7\nС какой целью производишь оценку своего будущего раритета? '
                                      'Короче, тебе вообще деньги нужны?', reply_markup=markup)


@bot.message_handler(commands=['start'])
def start(message):
    markup = types.ReplyKeyboardMarkup(resize_keyboard=True)
    item1 = types.KeyboardButton('🔸Что съесть?')
    item2 = types.KeyboardButton('🔸ДаркНет светлее!')
    item3 = types.KeyboardButton('🔸Даркнет темнее!')
    item4 = types.KeyboardButton('🔸Захребетник,отправь Донат')
    item5 = types.KeyboardButton('➡ Начать ART оценку')

    markup.add(item1, item2, item3, item4, item5)
    bot.send_message(message.chat.id, 'Чат-бот: "Профессиональный узкопрофильный сервис определения точной рыночной '
    'стоимости -СЮРРЕАЛ АРТ- объектов, еще перед их созданием"! Программа выдает точную рыночную стоимость произведения' 
    ' искусства в будущем, в границах 2030-2050гг. Сервис удобен тем, что еще перед созданием произведения искусства,'
    'художник способен оценить целесообразность своего проекта, с финансовой точки зрения! Сервис разработан, на благо'
    ' художников авангардистов! Программа способна облегчить, процесс принятия решений и сократить душевные терзания в '
    'случае их наличия!')
    time.sleep(3)
    bot.send_message(message.chat.id, 'Привет, {0.first_name}!'.format(message.from_user), reply_markup=markup)
    time.sleep(3)
    bot.send_message(message.chat.id, 'Комфортно располагайся Художник и будь как дома!')
    time.sleep(3)
    bot.send_message(message.chat.id, 'Посмотри, там внизу кнопки есть! Давай, начинай осваиваться!')

@bot.message_handler(commands=['art'])
def art(message):
    bot.send_message(message.chat.id, '.TimoninArtBot думает!')
    time.sleep(1)
    bot.send_message(message.chat.id, '...TimoninArtBot думает!')
    time.sleep(1)
    bot.send_message(message.chat.id, '.....TimoninArtBot думает!')
    time.sleep(1)
    bot.send_message(message.chat.id, '.......TimoninArtBot думает!')
    time.sleep(1)
    bot.send_message(message.chat.id, '.........TimoninArtBot думает!')
    time.sleep(1)
    bot.send_message(message.chat.id, '...........TimoninArtBot думает!')
    time.sleep(1)
    bot.send_message(message.chat.id, '.............TimoninArtBot думает!')
    time.sleep(3)
    bot.send_message(message.chat.id, 'После долгих и изнурительных подсчетов')
    time.sleep(3)
    bot.send_message(message.chat.id, 'Стоимость вашего сюрреал Арт объекта, в границах 2030-2050гг будет '
                                       'составлять сумму в размере:')
    time.sleep(5)
    bot.send_message(message.chat.id, str(random.randint(1000, 1000000)) + ' Рублей Европейской Земной '
                                       'Конфедерации!')
    time.sleep(5)
    bot.send_message(message.chat.id, 'Уважаемый Художник,мы гордимся вашим результатом! Вы можете получить хороший '
                                      'профит, если займетесь своим Проектом!')
    time.sleep(7)
    bot.send_message(message.chat.id, 'Сервис TimoninArtBot благодарит вас за доверие, окзанное нам! Мы и в дальнейшем '
    'будем работать на благо Сюрреал Арт Искусства! Продалжайте заниматься творчеством! Мы желаем вам вдохновения и '
    'поддержки, со стороны ваших близких!')
    time.sleep(7)
    bot.send_message(message.chat.id, 'Предлагаем вам произвести оценку еще одного задуманного произведения искусства, '
    'так же вы можете посмотреть советы на тему: "ЧТО СЕЙЧАС СЪЕСТЬ", так же вы можете поизменять освещение ДаркНет!'
    ' Воспользуйтесь соответствующим меню внизу экрана.')
    time.sleep(7)
    bot.send_message(message.chat.id, 'Отправляй Донат Манеро (XMR) и иди покушай - ты заслужил!!!')

@bot.message_handler(content_types=['text'])
def bot_message(message):
    if message.chat.type == 'private':
        if message.text == '🔸Что съесть?':
            eda=['Покушай кукурузки вареной!','Слопай банку тушенки!','Замни макарохи "По флотски"!',
                 'Просто водички попей!', 'Ничего, ты на диете!','На дармовщинку и уксус сладкий!',
                 'Покушай витамины - тебе для головы надо!','Хлеб всему голова!','Растягайчики сегодня удались!',
                 'Буженинка нынче в цене!','Упади лицом в салат!', 'Стащи в магазине батон колбасы!',
                 'Вылови морской капусты!','Приготовь себе омлет!','Ты уже все сожрал!','Вылови окунька из лужи!',
                 'Полижи сосульку!','Лучше книжку почитай про Питон!','Пробегись по полю конопли!',
                 'Погрызи сосновую шишку!','Попроси обед у полицейского!','Прикинься мышью - жри зернышки!',
                 'Сдай бутылки - купи бухло!','А что самому слабо придумать?']
            bot.send_message(message.chat.id, choice(eda))
        elif message.text == '🔸ДаркНет светлее!':
            svet=['Ужас, теперь ДаркНет намного светлее!', 'Молодец, сейчас на тебя копы наденут браслеты!',
                  'Поосторожней, ты оставляешь цифровой след!','Трояны теперь видны как на ладони!',
                  'Зачем так ярко? Нас спалили!','ДаркНет теперь уже совсем не тот!','И где теперь фармить?',
                  'Касперский теперь совсем оборзеет!','Бизнес теперь невозможен! Как с людьми договариваться?',
                  'ДаркНет потерял привлекательность!','Иди работать осветителем в театр, бездырь!',
                  'Не будь гадом, выключи свет, оставь все как было!','ДаркНет теперь не для свободных людей!',
                  'ДаркНет тепеь наводнила полиция!','Ты совершил нехороший поступок!',
                  'Кто тебя просил, не нажимай больше кнопки!',
                  'Не засовывай на спор, лампочку в рот - попадешь в травмапункт!', 'Потомки тебя придадут анафеме!',
                  'Я с тобой больше не разговариваю!','Отвратительное, непостижимое действие!']
            bot.send_message(message.chat.id, choice(svet))
        elif message.text == '🔸Даркнет темнее!':
            dark=['Ты спасаешь человечество!','Тьма придает нам сил!','Теперь мы натворим делов!',
                  'Комфортная атмосфера!','Спасибо, теперь намного проще!','Тебя не забудут потомки!',
                  'ДаркНет теперь привлекателен!','В ДарКет теперь как дома!', 'Теперь хочется дышать полной грудью!',
                  'Темнота друг молодежи!','ДаркНет привлекателен для инвестиций!', 'Где-то плачет Касперский!',
                  'ДаркНет комфортая среда!','Вот это вот - достойный поступок!','Тепеь будем искать черную кошку!',
                  'Теперь глаза разбегаются!','Сразу пооявились новые виды деятельности',
                  'В ДаркНет сразу появились рабочие места','СуперГуд! Пошли за пивом!',
                  'Полиция теперь осталась без работы - все ушли в ДаркНет!','Правильное решение! Теперь заживем!',
                  'Теперь ДаркНет как поле - сажай и окучивай!',
                  'Мы не держим медь в карманах - нас уважают в ресторанах!','Давай попробуем сделать еще потемнее!',
                  'И правильно, я предлагаю вообще все лампочки выкинуть!','Тьма - Зер Гуд!',
                  'Теперь можно корчить рожи - никто не увидит!','Теперь грязь не видна - можно не убираться',
                  'Начала происходить переоценка ценностей!','Пошли в Dos атаку!','Вирусняк теперь расплодится!',
                  'Поздравляю. ты теперь Ноунейм!']
            bot.send_message(message.chat.id, choice(dark))
        if message.text == '🔸Захребетник,отправь Донат':
            bot.send_message(message.chat.id, 'Отправь донат Сенсею, голубиной почтой, на адрес: World, '
                    'DarkNet, TimoninArtBot!')
            time.sleep(2)
            bot.send_message(message.chat.id, 'Здесь других вариантов событий нет, поэтому не надо неистово клацать '
                    'по этому пункту менюхи!)))')

        if message.text == '➡ Начать ART оценку':
            time.sleep(3)
            bot.send_message(message.chat.id, 'Всего будет 7 (семь) вопросов!')
            time.sleep(3)
            bot.send_message(message.chat.id, 'Художник, клацни тут: /s1')


@bot.callback_query_handler(func=lambda call: True)
def callback(call):
    l=['ОТЛИЧНЫЙ ОТВЕТ!','ИНТЕРЕСНОЕ МНЕНИЕ!','ПРАВИЛЬНЫЙ ВЫБОР!','ТЫ УВЕРЕН???','ПО ДРУГОМУ И БЫТЬ НЕ МОЖЕТ!',
       'ТЕБЯ ЗА ЯЗЫК НИКТО НЕ ТЯНУЛ!','ЗА СЛОВА ОТВЕЧАТЬ НАДО','ОХ КАК ТЫ ЗАГОВОРИЛ...','ГУСАРСКАЯ ТОЧКА ЗРЕНИЯ!',
       'САМ ДОГАДАЛСЯ?','ЗАЮЗАЛ ЧТО?ГДЕ?КОГДА?','РИСК БЛАГОРОДНОЕ ДЕЛО!','ОТВЕЧАЙ СМЕЛЕЕ!','НЕ ТУПИ!','СОБЕРИСЬ ТРЯПКА!',
       'НАУЧИСЬ ЩИ ВАРИТЬ!','БРЕД!','ОПА-ОПА-О-ПА-ПА!','НЕ БЕЗОБРАЗНИЧАЙ!','ПРОГИБ ЗАМЕЧЕН И ЗАСЧИТАН!',
       'ЯБЛОКО ОТ ЯБЛОНЬКИ...!','НЕ РИСУЙСЯ!','ЗДЕСЬ МОЖНО ПОСПОРИТЬ!','ТАКОЕ ТОЛЬКО ПО ТРЕЗВОМУ...!','ЁПРСТ ЁКЛМН!',
       'ШУТНИК ОДНАКО!','РАШАЙСЯ МАСТЕР!','ТЕБЕ НУЖЕН СОВЕТ?','БЛИН, КАК ВСЕГДА!','ИДИ ПРОСПИСЬ!','МИСТЕР ЛОГИКА!',
       'СРОЧНО ПРИЧЕШИСЬ!','ВЫПЕЙ ЯДУ!','ВО ТЫ ШЕЛЬМА!','САМОГОНЩИК ЧТО ЛИ?', 'УДАЛИ ЮТУБ!']
    bot.answer_callback_query(callback_query_id=call.id, text=choice(l))
    time.sleep(2)
    answer = ''

    if call.message:
        if call.data == 'z1':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Все с твоими делами '
            'понятно! Никто не сомневался в этом.\nДля продолжения клацни тут: /s2')
        elif call.data == 'z2':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Я думал ты похож на '
            'хвастунишку, а оказывается ты просто рисуешься! Художник - да ты нарцис!\nДля продолжения клацни тут: /s2')
        elif call.data == 'z3':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='После этого '
            'признания мы будем все гордиться тобой! Подойди к зеркалу и сделай вид что ты герой!\n'
             'Для продолжения клацни тут: /s2')
        elif call.data == 'z4':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Красафчек! '
            'Зашли криптовалюту Манеро (XMR) на мой адрес!\nДля продолжения клацни тут: /s2')


        elif call.data == 'z5':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Похвальная точка '
            'зрения! Ты выделяешся среди окружающих! Молодец!\nДля продолжения клацни тут: /s3')
        elif call.data == 'z6':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Такой ответ, '
            'призывает окружающих, снимать перед тобой шляпу!\nДля продолжения клацни тут: /s3')
        elif call.data == 'z7':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Талантливая оценка! '
             'Это даст свои плоды! Дерзай дальше!\nДля продолжения клацни тут: /s3')
        elif call.data == 'z8':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Не хочешь денег, '
            'пришей к попе веник! Не хочешь думать засылай криптовалюту '
            'Манеро (XMR) на мой адрес!\nДля продолжения клацни тут: /s3')


        elif call.data == 'z9':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Мамкин художник!'
            'Желаю успехов! Давай старайся!\nДля продолжения клацни тут: /s4')
        elif call.data == 'z10':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Я встану в очередь '
            'посмотреть на результат! Да ты умеешь удивлять!\nДля продолжения клацни тут: /s4')
        elif call.data == 'z11':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Что то мир вокруг '
            'напрягся! Скоро все ломанутся к тебе брать автограф!\nДля продолжения клацни тут: /s4')
        elif call.data == 'z12':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Безыдейное '
            'ты существо! Ждем криптовалюту Манеро (XMR) на мой адрес!\nДля продолжения клацни тут: /s4')


        elif call.data == 'z13':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Ты шаришб '
            'в поверхностях! Не останавливайся, продолжай исследования!\nДля продолжения клацни тут: /s5')
        elif call.data == 'z14':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Фантазия зашкаливает! '
            'Ты явно из особенных! Давай жги еще!\nДля продолжения клацни тут: /s5')
        elif call.data == 'z15':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Забавная точка зрения! '
            'Это явно даст хороший результат! Продолжай двигаться вперед!\nДля продолжения клацни тут: /s5')
        elif call.data == 'z16':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Ты никто и звать тебя '
            'никак! Забивай пароль и переводи криптовалюту Манеро (XMR) на мой адрес!\nДля продолжения клацни тут: /s5')


        elif call.data == 'z17':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Вот это по нашему! '
            'Ибо нефиг! Все правильно!\nДля продолжения клацни тут: /s6')
        elif call.data == 'z18':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Мы поддерживаем! '
            'Мы за! Это истинная точка зрения!\nДля продолжения клацни тут: /s6')
        elif call.data == 'z19':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Мы солидарны! '
            'Наши мысли сходятся! Мы думаем одинаково!\nДля продолжения клацни тут: /s6')
        elif call.data == 'z20':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Пошел ты нахрен '
            'со своей правильностью! Если не сделаешь платеж нам на кошелек, не будем ничего оценивать! '
            'Отправляй криптовалюту Манеро (XMR) на мой адрес!\nДля продолжения клацни тут: /s6')


        elif call.data == 'z21':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Да, да, да! '
            'Мы в одной команде! Можешь немного порулить!\nДля продолжения клацни тут: /s7')
        elif call.data == 'z22':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Хоть кто то думает '
            'о искусстве! Смотри не перестарайся!\nДля продолжения клацни тут: /s7')
        elif call.data == 'z23':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Вот это поворот! '
            'Буду следить за тобой! Все супер!\nДля продолжения клацни тут: /s7')
        elif call.data == 'z24':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Да ты не художник, '
            'ты трус! Будем с тобой вести себя по другому! Будем разговаривать с тобой через губу! Жду '
            'криптовалюту Манеро (XMR) на мой адрес!\nДля продолжения клацни тут: /s7')


        elif call.data == 'z25':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Я смотрю любишь ты '
            'пожрать! В здоровом теле здоровый дух! Продолжай нагуливать аппетит!\nДля продолжения клацни тут: /art')
        elif call.data == 'z26':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Вызывает уважение - '
            'когда желания реальны! Арт реализм дает свои плоды! Продолжаем мечтать '
            'и пускать слюни!\nДля продолжения клацни тут: /art')
        elif call.data == 'z27':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Что характерно - '
            'так это то, что мысли материальны! Мыслим глобально! Мыслим широко!\nДля продолжения клацни тут: /art')
        elif call.data == 'z28':
            bot.edit_message_text(chat_id=call.message.chat.id, message_id=call.message.id, text='Скучный ты! '
            'Не интересно с тобой! Гони криптовалюту Манеро (XMR) на мой адрес!\nДля продолжения клацни тут: /art')

bot.polling(none_stop = True)

