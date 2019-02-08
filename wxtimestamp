#!/bin/python

import datetime
from wxpy import *

bot = Bot(console_qr=True, cache_path=True)

'''
@bot.register()
def just_print(msg):
    #print mes
        print(msg)
        msg.reply(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
'''

#群聊中仅针对@平头哥且输入t的消息回复时间戳
@bot.register(Group, TEXT)
def print_group_msg(msg):
        if msg.is_at and msg.text == '@平头哥 t':
        #if msg.is_at and msg.text == 't':
                print(msg.text)
                msg.reply(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))

#堵塞消息
embed()
