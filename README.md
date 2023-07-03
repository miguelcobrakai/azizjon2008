class Ota:
    def init(self,ism ,familiya,yili):
        self.ism = ism
        self.familiya = familiya
        self.yili = yili

    def get_info(self):
        info = f"{self.ism} {self.familiya}. "
        info += f"{self.yili}- yilda tug'ilgan "
        return  info

    def get_age(self,yil):
        return yil - self.yili

class Bola(Ota):
    def init(self,ism,familiya,yili,idraqami,fanlar):
        super().init(ism,familiya,yili)
        self.idraqami = idraqami
        self.fanlar = fanlar

    def get_id(self):
        return self.idraqami


class Fanlar:
    def init(self,jismoniy, huquq, english , tarbiya):
        self.jismoniy = jismoniy
        self.huquq = huquq
        self.english = english
        self.tarbiya = tarbiya

    def get_fanlar(self):
        fanlar = f"{self.jismoniy} {self.huquq}"
        fanlar += f"{self.english} {self.tarbiya}"
        return fanlar

bola_fanlar = Fanlar("jismoniy", "huquq " , "english", "tarbiya")
bola = Bola("azizjon", "abdumalikov", 2000, "D87008836",bola_fanlar)
print(bola.fanlar.get_fanlar())  ![image](https://github.com/miguelcobrakai/azizjon2008/assets/138461360/56a13cc4-00c0-4479-a0a9-8a60aea11a5c)

