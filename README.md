### Under-Check

  - [ ] [geekcomputers](https://github.com/geekcomputers/Python)

### [Binding](https://wiki.python.org/moin/IntegratingPythonWithOtherLanguages)

  - [ ] [c-in-python](https://stackoverflow.com/questions/13990317/generate-python-bindings-what-methods-programs-to-use)
  
       keyword :  wrapper,[extending](https://docs.python.org/3/extending/extending.html),binding,calling,[integrating](https://wiki.python.org/moin/IntegratingPythonWithOtherLanguages),[embedding](https://docs.python.org/2/extending/embedding.html),python,c++ 
        
      * [ctypes](https://docs.python.org/2/library/ctypes.html)
      * [swig](https://github.com/swig/swig)[tutorial](http://www.swig.org/tutorial.html)
      * [boost.python](http://www.boost.org/doc/libs/1_49_0/libs/python/doc/)
      * [cython]()
      
  - [ ] [ipc](http://zguide.zeromq.org/)
      
      * [zeromq:one and only ipc between python and c++](https://github.com/zeromq/pyzmq)
      * [zguide](https://github.com/booksbyus/zguide/tree/master/examples)
      * [libzmq](https://github.com/zeromq/libzmq)
      
      * [clif](https://github.com/google/clif)
      
  - [x] [python-in-c](https://github.com/gustavkkk/embedding-python-in-c)
  
### Conversion

  - [x] [chinese2Integer](https://github.com/gustavkkk/python-small-module/blob/master/chn2int.py)
  
  - [ ] [csv2sqlite](https://github.com/rasbt/python_reference/blob/master/useful_scripts/large_csv_to_sqlite.py)
  
  - [ ] [cpp2python](https://github.com/andreikop/cpp2python)
  
  - [ ] [python2android](https://github.com/kivy/python-for-android)
  
  - [ ] [shell-command-in-python](https://github.com/amoffat/sh)
  
### Auto

  - [x] [wechat](https://github.com/littlecodersh/ItChat)
  
        import itchat
        itchat.auto_login()
        author = itchat.search_friends(nickName='田')[0]
        author.send('greeting, littlecoder!')
   
  - [ ] [QQ](https://github.com/pandolia/qqbot)
  
  - [ ] [twitter](https://github.com/tweepy/tweepy)
  
  - [x] email
  
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
     
  - [x] [ui](https://gfycat.com/PointlessSimplisticAmericanquarterhorse)
  
         import pyautogui
         import time
         pyautogui.position()
         while True:
           time.sleep(0.1)
           pyautogui.click(15,42)
           
  - [ ] [slacker](https://github.com/os/slacker)
  
  - [ ] [skype](https://github.com/Skype4Py/Skype4Py)
  
  - [ ] [chrome-db](https://github.com/MonroCoury/Forensic-Tools)
  
  - [ ] Amazon
      * [boto](https://github.com/boto/boto)
      * [aws-cli](https://github.com/aws/aws-cli)
  
  - [ ] [Trading](https://github.com/quantopian/zipline) : [tushare:historical-data-from-chinese-stock](https://github.com/waditu/tushare)
### Data & Time

  - [ ] [arrow](https://github.com/crsmithdev/arrow)
  
### File/Dir Processing

### NLP

  - [ ] [spacy](https://spacy.io/) : [src](https://github.com/explosion/spaCy) : [models](https://github.com/explosion/spacy-models/)
  
        import spacy
        nlp = spacy.load('en')
        doc1 = nlp(u'the fries were gross')
        doc2 = nlp(u'worst fries ever')
        doc1.similarity(doc2)
        
  - [x] [gensim](https://github.com/RaRe-Technologies/gensim)
  
       * [tutorials](https://github.com/RaRe-Technologies/gensim/blob/develop/tutorials.md)
       * [doc2vec](https://github.com/RaRe-Technologies/gensim/blob/develop/docs/notebooks/doc2vec-lee.ipynb)
       * [summarization](https://github.com/RaRe-Technologies/gensim/blob/develop/docs/notebooks/summarization_tutorial.ipynb)
       
  - [ ] [newspaper](https://github.com/codelucas/newspaper)

  - [ ] [TextBlob](https://github.com/sloria/TextBlob)
  
 ### Utility
 
  - [x] [magic-wormhole:file-send-receiver](https://github.com/warner/magic-wormhole)
   
        $ pip install magic-wormhole
        
        sender$ wormhole send README.md
              Sending 7924 byte file named 'README.md'
              On the other computer, please run: wormhole receive
              Wormhole code is: 7-crossover-clockwork
        receiver$ wormhole receive
                Enter receive wormhole code: 7-crossover-clockwork
                Receiving file (7924 bytes) into: README.md
                ok? (y/n): y
  - [ ] [maybe:check-before-done](https://github.com/p-e-w/maybe)
  
        $ pip install maybe
        
  - [ ] [howdoi:programming-grammar-check](https://github.com/gleitz/howdoi)
  
        $ pip install howdoi
        
  - [ ] [glances:An-eye-on-your-system](https://github.com/nicolargo/glances)
  
        $ pip install glances
        $ glance
        
  - [x] [thefuck:Auto-Correcting-Command](https://github.com/nicolargo/glances)
  
  - [ ] [fabric:Shell-Command-On-Multi-Servers-Same-Time](https://github.com/fabric/fabric)
  
  - [ ] [fire:Automatically-generating-CLIs-from-any-Python-Object](https://github.com/google/python-fire)
  
        import fire
        class Calculator(object):
          """A simple calculator class."""
          def double(self, number):
            return 2 * number
        if __name__ == '__main__':
          fire.Fire(Calculator)
        
        $ python calculator.py double 10  # 20
        $ python calculator.py double --number=15  # 30
       
  - [ ] [mackup:Back-Up-Application-Setting-Into-DropBox](https://github.com/lra/mackup)
  
  - [ ] [mkdocs:Make-Project-Docs](https://github.com/mkdocs/mkdocs)
  
  - [ ] [BossSensor:Hide-screen-when-boss-is-approaching](https://github.com/Hironsan/BossSensor)
  
  - [ ] [moviepy:Video-Editing](http://zulko.github.io/moviepy/)
  
  - [ ] [legit:Git-for-Humans](https://github.com/kennethreitz/legit)
  
  - [ ] [wttr:weather](https://github.com/chubin/wttr.in)
  
  - [ ] [voltron:reversing-tool](https://github.com/snare/voltron)
  
 ### [Python in C++](https://www.coveros.com/calling-python-code-from-c/)
 
 
 ### [Distribution](https://stackoverflow.com/questions/14165398/a-good-python-to-exe-compiler)
 
  - [x] [pyinstaller](https://github.com/pyinstaller/pyinstaller)
  
        This is the one and only choice for tensorflow-based application distribution and works great. But, you have to install python using brew not anaconda for Mac.
        
        $ pyinstaller  --onefile --windowed xxx.py
        $ pyinstaller xxx.spec
        
  - [x] [cx_Freeze](https://github.com/anthony-tuininga/cx_Freeze/blob/master/doc/distutils.rst)
  
        import sys
        from cx_Freeze import setup, Executable
        build_exe_options = {"packages": ["os"], "excludes": ["tkinter"]}
        base = None
        if sys.platform == "win32":
            base = "Win32GUI"

        setup(  name = "guifoo",
                version = "0.1",
                description = "My GUI application!",
                options = {"build_exe": build_exe_options},
                executables = [Executable("guifoo.py", base=base)])
 
  ### GUI 
  - [ ] [pyqt]()
  
  - [ ] [kivy]()

  ### Bot
  - [ ] ChatBot
    
      * [ChatterBot](https://github.com/gunthercox/ChatterBot)
      
  - [ ] WeChat
      
      * [WeixinBot](https://github.com/Urinx/WeixinBot)

  ### Web
  
  - [ ] [wsgi](http://wsgi.readthedocs.io/en/latest/frameworks.html）
  
  - [ ] [webpy](https://github.com/webpy/webpy)
      
        "Django lets you write web apps in Django. TurboGears lets you write web apps in TurboGears. Web.py lets you write web apps in Python."
          —  Adam Atlas
          
        $ pip install web.py
        
        import web
        urls = ( '/(.*)', 'hello')
        app = web.application(urls, globals())
        class hello:  
          def GET(self, name):
            if not name: 
              name = 'World'
            return 'Hello, ' + name + '!'
        if __name__ == "__main__":
          app.run()
          
  - [ ] [falcon](https://github.com/falconry/falcon)
    
  - [ ] [aiohttp:Client/Server](https://github.com/aio-libs/aiohttp)
  
  ### Django-Case
  
  - [ ] [NewsBlur:Read-News-From-Variable-Sources](https://github.com/samuelclay/NewsBlur)
  
  
  ### 3D
  
  - [ ] [SpaceshipGenerator:with-Random-Seed](https://github.com/a1studmuffin/SpaceshipGenerator)
  
  
  ### Computer Vision
  
  - [ ] [srez:super-resolution-16x16to64x64-face](https://github.com/david-gpu/srez)
  
  ### Prediction
  
  - [ ] [prophet](https://github.com/facebook/prophet) : [Quick-Start](https://facebook.github.io/prophet/docs/quick_start.html#python-api)
  
        import pandas as pd
        import numpy as np
        from fbprophet import Prophet
        df = pd.read_csv('../examples/example_wp_peyton_manning.csv')
        df['y'] = np.log(df['y'])
        df.head()
        m = Prophet()
        m.fit(df)

