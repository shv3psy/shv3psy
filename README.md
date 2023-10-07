проблема. я написал обработчик команды старт для телеграм бота на aiogram, который должен присылать сообщения с инлайн кнопкой, оно работает, но когда пишу /start в группе, сообщение бот кидает в лс. помогите пж

@dp.message_handler(commands=["start"])
async def vote_command(message: types.Message):
    #ikb.add(ib20)
    #ikb = InlineKeyboardMarkup(row_width=2)
    #ib20 = InlineKeyboardButton(text=text',
    #                       url='https://text')
    await bot.send_photo(chat_id=message.from_id,
                         photo="https://photo.jpg",
                         caption=f'text',
                         reply_markup=ikb)

