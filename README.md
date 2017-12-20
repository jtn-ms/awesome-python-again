### Conversion

  - [ ] [chinese2Integer](https://github.com/gustavkkk/python-small-module/blob/master/chn2int.py)
  
  - [ ] [csv2sqlite](https://github.com/rasbt/python_reference/blob/master/useful_scripts/large_csv_to_sqlite.py)

### Auto

  - [ ] [wechat](https://github.com/littlecodersh/ItChat)
  
        import itchat
        itchat.auto_login()
        author = itchat.search_friends(nickName='田')[0]
        author.send('greeting, littlecoder!')
   
  - [ ] [QQ](https://github.com/pandolia/qqbot)
  
  - [ ] email
  
     * [gmail-receiver](https://github.com/charlierguo/gmail):[gmail-sender](https://github.com/paulchakravarti/gmail-sender)
     
            import gmail
            from gmail import Gmail
            g = gmail.login(username, password)
            
     * [mailthon](https://github.com/eugene-eeo/mailthon)
     
            from mailthon import postman, email
            p = postman(host='smtp.outlook.com', auth=('username', 'password'))
            r = p.send(email(
                content=u'<p>Hello 世界</p>',
                subject='Hello world',
                sender='Pi<gustav0125@outlook.com>',
                receivers=['doe@163.com']))
                assert r.ok
     
     * [gmail-receiver]()
     
  - [ ] [ui](https://gfycat.com/PointlessSimplisticAmericanquarterhorse)
  
         import pyautogui
         import time
         pyautogui.position()
         while True:
           time.sleep(0.1)
           pyautogui.click(15,42)
           
  - [ ] [slacker](https://github.com/os/slacker)
  
  - [ ] [skype](https://github.com/Skype4Py/Skype4Py)
  
  - [ ] [chrome-db](https://github.com/MonroCoury/Forensic-Tools)
  
  - [ ] [Amazon]()
  
  - [ ] [Trading]()
   
### File/Dir Processing

###
