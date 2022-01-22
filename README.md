# PyxelButtonManager

## Example
"""
import PyxelButton as pb
class APP:
  def __init__(self):
    pyxel.init(...)
    pyxel.mouse(True)
    
    def function_a():
      print("Pushed Button_A")
    button_a : pb.BaseButton = pb.TextButton(x=0,y=0,s="Button_A",col=pyxel.COLOR_BLACK,func=lambda:function_a())
    
    def function_b():
      print("Pushed Button_B")
    button_b : pb.BaseButton = pb.TextButton(x=0,y=10,s="Button_B",col=pyxel.COLOR_BLACK,func=lambda:function_b())
    
    self.buttonManager = pb.ButtonManager(buttons=[[button_a,lambda:TRUE,[pyxel.SPACE], [button_b,lambda:TRUE,[]]]])
    
    pyxel.run(self.update, self.draw)
  def update(self):
    ...
    self.buttonManager.update()
  
  def draw(self):
    ...
    self.buttonManager.draw()
    
APP()
"""
