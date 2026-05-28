# 🚀 Como Rodar o Projeto - Passo a Passo

## 1️⃣ Abra o Terminal
- No Mac, pressione `Cmd + Espaço` e digite "Terminal"
- Ou abra o terminal integrado do VS Code

## 2️⃣ Navegue até a pasta do projeto
```bash
cd /Users/hellenruthes/dev/mr1_hc_utfpr
```

## 3️⃣ Instale as dependências
```bash
pip3 install -r requirements.txt
```

## 4️⃣ Crie a pasta de resultados
```bash
mkdir -p result
```

## 5️⃣ Rode o programa principal
```bash
python3 main.py
```

---

## 📝 Comandos Opcionais

### Se quiser rodar com parâmetros personalizados:
```bash
python3 main.py --train dataset/MR-MS-new/P0001/ --nifti_train result/P0001.nii.gz
```

### Se quiser desabilitar a visualização (mais rápido):
```bash
python3 main.py --visualize 0
```

### Se quiser ver o progresso detalhado:
```bash
python3 main.py --debug_progress 1
```

---

## ⚠️ Problemas Comuns

### Erro: "No module named 'pydicom'"
```bash
pip3 install pydicom==2.3.0
```

### Erro: "No such file or directory: 'result/'"
```bash
mkdir -p result
```

### Erro: "No module named 'torch'"
```bash
pip3 install torch torchvision
```

---

## 🎯 Resumo Rápido (Cole tudo de uma vez)
```bash
cd /Users/hellenruthes/dev/mr1_hc_utfpr
pip3 install -r requirements.txt
mkdir -p result
python3 main.py
```
