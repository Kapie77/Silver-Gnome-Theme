![silver1](https://i.ibb.co/Q3vYc8ft/screenshot.png)

# COMO INSTALAR O TEMA

## EXTENSÕES NECESSÁRIAS
Para instalar temas no Gnome, você precisa de algumas extensões que podem ser baixadas aqui: https://extensions.gnome.org/
- [Install Browser Extension](https://extensions.gnome.org/) - Permite instalar extensões através do seu navegador.
- [User Themes](https://extensions.gnome.org/extension/19/user-themes/) - Carrega temas do shell a partir do diretório do usuário (ou seja, via pastas do seu computador).
- Gnome Tweaks - Você precisa desta ferramenta para gerenciar temas. Instale-a através da loja da sua distro ou digite o seguinte no terminal: ```sudo apt install gnome-tweaks```
- [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) - Permite colocar uma imagem de fundo na tela de bloqueio.
- [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/) - Permite personalizar a dock.

## INSTALANDO O TEMA
Instale todas as extensões necessárias acima.

Vá para a pasta “home” e pressione Ctrl + H para visualizar as pastas ocultas (ou marque a opção para visualizar pastas ocultas) e crie uma pasta chamada **.themes** e **.icons**.

Extraia o arquivo .zip do tema, copie a pasta extraída e cole-a em .themes.

Abra o Gnome Tweaks, vá para Aparência e, em “Aplicativos” e “Shell”, selecione **SilverTheme**, depois pressione Alt + F2 para reiniciar o shell e o tema estará instalado.

### COMO ALTERAR A COR E TAMANHO DA DOCK
Para alterar a cor do dock, abra Extensões, clique em “Configurações” em “Dash to Dock”, vá para “Aparência” e em “Personalizar a cor do dash” insira a cor #0fc0fc.

Para mudar o tamanho vá em "Position and size" e em "Icon size limit" coloque 32px.

Para mudar a opacidade vá em "Appearance" e em "Customize opacity" coloque 80%.

### COMO INSTALAR O PAPEL DE PAREDE
Instale a extensão [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) no site Gnome Extensions. Pressione a tecla super e abra o aplicativo Extensões. Em Lock Screen Background, clique em Configurações, selecione o papel de parede e pronto.
As imagens a serem usadas como papéis de parede estão na pasta “images”.

### COMO INSTALAR O TEMA DOS ICONES
Instale o tema de icones “Captiva-2”: https://www.gnome-look.org/p/1511577

### COMO INSTALAR O TEMA DO CURSOR
Instale o tema de cursor "Twilight cursors": https://www.gnome-look.org/p/1607387

### COMO FAZER APARECER NOTIFICAÇÕES PARA TESTE
Digite o comando abaixo no terminal e uma notifiação falsa irá aparecer.
<br>
```notify-send "Título" "Mensagem de Teste"```

### COMO TIRAR SCREENSHOT DE QUALQUER AREA (COMO LOCKSCREEN E TELA DO PRINT)
Digite o comando abaixo no terminal e um print será tirado dentro de 10 segundos:
<br>
```gnome-screenshot -d 10```

### THEME COLORS

| Color | Hex |  
|-----|------|
| Verde principal | #0ee6a7 | 
| Cinza principal | #cdd2d1| 
| Cinza em RGB transparente | rgba(205,210,209, 0.8) |
| Branco meio cinza em RGB transparente | rgba(255,255,255,0.91) |
| Verde escuro | #096d49 | 
| Verde/azul mais claro (da luva dele) | #4bfffe |
| Branco do panel | rgba(255,255,255,0.75) | 

<br>
```switch:checked { /* Cor do switch (o botão de on e off) */```
<br>
A cor azul quando clica com o botão direito na area de trabalha e passa o mouse em cima das opções está em:
```menu menuitem:hover, .menu menuitem:hover, .context-menu menuitem:hover {```
<br>
/* Cor das bolinhas pra marcar uma opção (tipo no settings -> fonts e tem umas opções lá pra marcar bolinha */
```check:checked, radio:checked {```
<br>
A cor azul quando clica em settings, por exemplo, e a opção clicada tem uma cor de fundo está em:
```row.activatable:selected {```
<br>
e aqui:
```.view:selected:focus, .view:selected, .view text:selected:focus, textview text:selected:focus, .view text:selected, textview text:selected, iconview:selected:focus, iconview:selected, flowbox flowboxchild:selected, modelbutton.flat:selected, .menuitem.button.flat:selected, treeview.view:selected:focus, treeview.view:selected, row:selected, calendar:selected {```
<br>
/* Botões de escolha tipo Left or Right do Settings -> Window Titlebars */
```notebook > header > tabs > arrow:checked, button:checked {```
