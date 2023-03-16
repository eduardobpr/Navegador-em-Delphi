unit Ubrowser;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, OleCtrls, SHDocVw, StdCtrls, Buttons, ExtCtrls, WinSkinData;

type
  TForm1 = class(TForm)
    Panel1: TPanel;
    Panel2: TPanel;
    SpeedButton1: TSpeedButton;
    SpeedButton2: TSpeedButton;
    SpeedButton3: TSpeedButton;
    SpeedButton4: TSpeedButton;
    ComboBox1: TComboBox;
    SpeedButton5: TSpeedButton;
    ComboBox2: TComboBox;
    Label1: TLabel;
    SpeedButton6: TSpeedButton;
    ir: TBitBtn;
    ir2: TBitBtn;
    Web: TWebBrowser;
    OpenDialog1: TOpenDialog;
    SpeedButton7: TSpeedButton;
    SkinData1: TSkinData;
    procedure SpeedButton5Click(Sender: TObject);
    procedure SpeedButton6Click(Sender: TObject);
    procedure SpeedButton1Click(Sender: TObject);
    procedure SpeedButton4Click(Sender: TObject);
    procedure SpeedButton2Click(Sender: TObject);
    procedure SpeedButton3Click(Sender: TObject);
    procedure SpeedButton7Click(Sender: TObject);
    procedure irClick(Sender: TObject);
    procedure ir2Click(Sender: TObject);
    procedure ComboBox1KeyDown(Sender: TObject; var Key: Word;
      Shift: TShiftState);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.dfm}

procedure TForm1.SpeedButton5Click(Sender: TObject);
begin
 if OpenDialog1.Execute then
    Begin
       ComboBox1.Items.LoadFromFile(OpenDialog1.FileName);
       ShowMessage('A lista foi carregada com sucesso!');
    end;
end;

procedure TForm1.SpeedButton6Click(Sender: TObject);
begin
 if OpenDialog1.Execute then
    Begin
       ComboBox2.Items.LoadFromFile(OpenDialog1.FileName);
       ShowMessage('A lista de Exploit Carregada!');
    end;
end;

procedure TForm1.SpeedButton1Click(Sender: TObject);
begin
 Web.GoBack;
end;

procedure TForm1.SpeedButton4Click(Sender: TObject);
begin
 Web.GoForward;
end;

procedure TForm1.SpeedButton2Click(Sender: TObject);
begin
 Web.Stop;
end;

procedure TForm1.SpeedButton3Click(Sender: TObject);
begin
 Web.Refresh;
end;

procedure TForm1.SpeedButton7Click(Sender: TObject);
begin
 Web.GoHome;
end;

procedure TForm1.irClick(Sender: TObject);
begin
 Web.Navigate(ComboBox1.Text+ComboBox2.Text);
end;

procedure TForm1.ir2Click(Sender: TObject);
begin
 ComboBox1.Items.Delete(0);
 ComboBox1.Items := ComboBox1.Items;
 Web.Navigate(ComboBox1.Text+ComboBox2.Text);
end;

procedure TForm1.ComboBox1KeyDown(Sender: TObject; var Key: Word;
  Shift: TShiftState);
begin
  if key = VK_RETURN then
  ir.Click;

end;

end.
