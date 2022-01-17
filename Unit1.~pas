unit Unit1;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, ExtCtrls, sPanel, StdCtrls, sComboBox, sSkinManager, sButton,
  acPNG, acImage, sMemo, DosCommand, ShellApi, Inifiles, sEdit, sGroupBox,
  acPathDialog;

type
  TForm1 = class(TForm)
    sSkinManager1: TsSkinManager;
    sPanel1: TsPanel;
    Note: TsMemo;
    DosCommand1: TDosCommand;
    sGroupBox1: TsGroupBox;
    edPak: TsEdit;
    edSig: TsEdit;
    Save: TsButton;
    Load: TsButton;
    OpenDialog1: TOpenDialog;
    btnPak: TsButton;
    btnSig: TsButton;
    sGroupBox2: TsGroupBox;
    edLivePaks: TsEdit;
    SaveLive: TsButton;
    LoadLive: TsButton;
    LivePaks: TsButton;
    sGroupBox3: TsGroupBox;
    cbBahasa: TsComboBox;
    Jalan: TsButton;
    Copy: TsButton;
    sPathDialog1: TsPathDialog;
    Hapus: TsButton;
    edRiotClient: TsEdit;
    RiotClient: TsButton;
    procedure JalanClick(Sender: TObject);
    procedure CopyClick(Sender: TObject);
    procedure LoadClick(Sender: TObject);
    procedure SaveClick(Sender: TObject);
    procedure HapusClick(Sender: TObject);
    procedure btnPakClick(Sender: TObject);
    procedure btnSigClick(Sender: TObject);
    procedure SaveLiveClick(Sender: TObject);
    procedure LivePaksClick(Sender: TObject);
    procedure LoadLiveClick(Sender: TObject);
    procedure RiotClientClick(Sender: TObject);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.dfm}

procedure TForm1.JalanClick(Sender: TObject);
begin
//ShellExecute(Handle, 'open', 'D:\Netgame\Riot Games\Riot Client\RiotClientServices.exe', '--launch-product=valorant --launch-patchline=live', nil, SW_SHOWNORMAL) ;
shellexecute(handle,'open',PChar('D:\Netgame\Riot Games\Riot Client\RiotClientServices.exe'),PChar(' --launch-product=valorant --launch-patchline=live'),NIL,SW_SHOWNORMAL);
end;

procedure TForm1.CopyClick(Sender: TObject);
begin
 if cbBahasa.text = 'ARAB' then begin
   Note.Clear;
   DeleteFile(edLivePaks.Text+ '\ar_AE_Text-WindowsClient.pak');
   DeleteFile(edLivePaks.Text+ '\ar_AE_Text-WindowsClient.sig');
   Note.Lines.Add('Original ar_AE_Text-WindowsClient.pak success deleted');
   Note.Lines.Add('Original ar_AE_Text-WindowsClient.sig success deleted');
   Note.Lines.Add('=====================================================');
   CopyFile(PChar(edPak.Text), PChar(edLivePaks.Text+ '\ar_AE_Text-WindowsClient.pak'), True);
   CopyFile(PChar(edSig.Text), PChar(edLivePaks.Text+ '\ar_AE_Text-WindowsClient.sig'), True);
   Note.Lines.Add('ENG version ar_AE_Text-WindowsClient.pak success copy');
   Note.Lines.Add('ENG version ar_AE_Text-WindowsClient.sig success copy');
   Note.Lines.Add('=====================================================');
 end;
 if cbBahasa.text = 'DEUTSCH' then begin
   Note.Clear;
   DeleteFile(edLivePaks.Text+ '\de_DE_Text-WindowsClient.pak');
   DeleteFile(edLivePaks.Text+ '\de_DE_Text-WindowsClient.sig');
   Note.Lines.Add('Original de_DE_Text-WindowsClient.pak success deleted');
   Note.Lines.Add('Original de_DE_Text-WindowsClient.sig success deleted');
   Note.Lines.Add('=====================================================');
   CopyFile(PChar(edPak.Text), PChar(edLivePaks.Text+ '\de_DE_Text-WindowsClient.pak'), True);
   CopyFile(PChar(edSig.Text), PChar(edLivePaks.Text+ '\de_DE_Text-WindowsClient.sig'), True);
   Note.Lines.Add('ENG version de_DE_Text-WindowsClient.pak success copy');
   Note.Lines.Add('ENG version de_DE_Text-WindowsClient.sig success copy');
   Note.Lines.Add('=====================================================');
 end;
 if cbBahasa.text = 'JAPAN' then begin
   Note.Clear;
   DeleteFile(edLivePaks.Text+ '\ja_JP_Text-WindowsClient.pak');
   DeleteFile(edLivePaks.Text+ '\ja_JP_Text-WindowsClient.sig');
   Note.Lines.Add('Original ja_JP_Text-WindowsClient.pak success deleted');
   Note.Lines.Add('Original ja_JP_Text-WindowsClient.sig success deleted');
   Note.Lines.Add('=====================================================');
   CopyFile(PChar(edPak.Text), PChar(edLivePaks.Text+ '\ja_JP_Text-WindowsClient.pak'), True);
   CopyFile(PChar(edSig.Text), PChar(edLivePaks.Text+ '\ja_JP_Text-WindowsClient.sig'), True);
   Note.Lines.Add('ENG version ja_JP_Text-WindowsClient.pak success copy');
   Note.Lines.Add('ENG version ja_JP_Text-WindowsClient.sig success copy');
   Note.Lines.Add('=====================================================');
 end;
 if cbBahasa.text = 'KOREAN' then begin
   Note.Clear;
   DeleteFile(edLivePaks.Text+ '\ko_KR_Text-WindowsClient.pak');
   DeleteFile(edLivePaks.Text+ '\ko_KR_Text-WindowsClient.sig');
   Note.Lines.Add('Original ko_KR_Text-WindowsClient.pak success deleted');
   Note.Lines.Add('Original ko_KR_Text-WindowsClient.sig success deleted');
   Note.Lines.Add('=====================================================');
   CopyFile(PChar(edPak.Text), PChar(edLivePaks.Text+ '\ko_KR_Text-WindowsClient.pak'), True);
   CopyFile(PChar(edSig.Text), PChar(edLivePaks.Text+ '\ko_KR_Text-WindowsClient.sig'), True);
   Note.Lines.Add('ENG version ko_KR_Text-WindowsClient.pak success copy');
   Note.Lines.Add('ENG version ko_KR_Text-WindowsClient.sig success copy');
   Note.Lines.Add('=====================================================');
 end;
 if cbBahasa.text = 'POLSKI' then begin
   Note.Clear;
   DeleteFile(edLivePaks.Text+ '\pl_PL_Text-WindowsClient.pak');
   DeleteFile(edLivePaks.Text+ '\pl_PL_Text-WindowsClient.sig');
   Note.Lines.Add('Original pl_PL_Text-WindowsClient.pak success deleted');
   Note.Lines.Add('Original pl_PL_Text-WindowsClient.sig success deleted');
   Note.Lines.Add('=====================================================');
   CopyFile(PChar(edPak.Text), PChar(edLivePaks.Text+ '\pl_PL_Text-WindowsClient.pak'), True);
   CopyFile(PChar(edSig.Text), PChar(edLivePaks.Text+ '\pl_PL_Text-WindowsClient.sig'), True);
   Note.Lines.Add('ENG version pl_PL_Text-WindowsClient.pak success copy');
   Note.Lines.Add('ENG version pl_PL_Text-WindowsClient.sig success copy');
   Note.Lines.Add('=====================================================');
 end;
 if cbBahasa.text = 'RUSSIAN' then begin
   Note.Clear;
   DeleteFile(edLivePaks.Text+ '\ru_RU_Text-WindowsClient.pak');
   DeleteFile(edLivePaks.Text+ '\ru_RU_Text-WindowsClient.sig');
   Note.Lines.Add('Original ru_RU_Text-WindowsClient.pak success deleted');
   Note.Lines.Add('Original ru_RU_Text-WindowsClient.sig success deleted');
   Note.Lines.Add('=====================================================');
   CopyFile(PChar(edPak.Text), PChar(edLivePaks.Text+ '\ru_RU_Text-WindowsClient.pak'), True);
   CopyFile(PChar(edSig.Text), PChar(edLivePaks.Text+ '\ru_RU_Text-WindowsClient.sig'), True);
   Note.Lines.Add('ENG version ru_RU_Text-WindowsClient.pak success copy');
   Note.Lines.Add('ENG version ru_RU_Text-WindowsClient.sig success copy');
   Note.Lines.Add('=====================================================');
 end;
end;

procedure TForm1.LoadClick(Sender: TObject);
  var load : TIniFile;
begin
  load := TIniFile.Create(ExtractFilePath(Application.ExeName)+'etc\valorant.ini');
  with load do begin
  edPak.Text := ReadString('MAINENGS','PAK', edPak.Text);
  edSig.Text := ReadString('MAINENGS','SIG',edSig.Text);
 end
end;

procedure TForm1.SaveClick(Sender: TObject);
var save : TIniFile;
begin
 save := TIniFile.Create(ExtractFilePath(Application.ExeName)+'etc\valorant.ini');
  with save do begin
  WriteString('MAINENGS','PAK',(edPak.Text));
  WriteString('MAINENGS','SIG',(edSig.Text));
 end
end;

procedure TForm1.HapusClick(Sender: TObject);
begin
DeleteFile('D:\Netgame\Riot Games\VALORANT\live\ShooterGame\Content\Paks\en_US_Text-WindowsClient.pak');
DeleteFile('D:\Netgame\Riot Games\VALORANT\live\ShooterGame\Content\Paks\en_US_Text-WindowsClient.sig');
Note.Lines.Add('en_US_Text-WindowsClient.pak success deleted');
Note.Lines.Add('en_US_Text-WindowsClient.sig success deleted');
end;

procedure TForm1.btnPakClick(Sender: TObject);
begin
if OpenDialog1.Execute then
  begin
    edPak.Text:=OpenDialog1.FileName;
  end;
end;

procedure TForm1.btnSigClick(Sender: TObject);
begin
if OpenDialog1.Execute then
  begin
    edSig.Text:=OpenDialog1.FileName;
  end;
end;

procedure TForm1.SaveLiveClick(Sender: TObject);
var save : TIniFile;
begin
 save := TIniFile.Create(ExtractFilePath(Application.ExeName)+'etc\valorant.ini');
  with save do begin
  WriteString('VALORANT LIVE','PAKSDIR',(edLivePaks.Text));
  WriteString('RIOT GAME','RIOTCLIENDIR',(edRiotClient.Text));
 end
end;

procedure TForm1.LivePaksClick(Sender: TObject);
begin
if sPathDialog1.Execute then
  begin
    edLivePaks.Text:=sPathDialog1.Path;
  end;
end;

procedure TForm1.LoadLiveClick(Sender: TObject);
  var load : TIniFile;
begin
  load := TIniFile.Create(ExtractFilePath(Application.ExeName)+'etc\valorant.ini');
  with load do begin
  edLivePaks.Text := ReadString('VALORANT LIVE','PAKSDIR', edLivePaks.Text);
  edRiotClient.Text := ReadString('RIOT GAME','RIOTCLIENDIR', edRiotClient.Text);
 end
end;

procedure TForm1.RiotClientClick(Sender: TObject);
begin
if sPathDialog1.Execute then
  begin
    edRiotClient.Text:=sPathDialog1.Path;
  end;
end;

end.
