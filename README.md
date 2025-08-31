# TASK-No.1
# News Topic Classifier Using BERT

🎯 Objective  
Fine-tune a transformer model (**bert-base-uncased**) to classify news headlines into topic categories using the AG News dataset.  
This project demonstrates the end-to-end NLP pipeline: preprocessing, model fine-tuning, evaluation, and lightweight deployment.

---

📊 Dataset  
**Source:** AG News Dataset – Hugging Face  
**Auto-downloaded** by the training script (no manual file required)  

**Structure:**  
- `text`: News headline or short description  
- `label`: Target variable (topic class: 0–3)  

**Categories:**  
1. World  
2. Sports  
3. Business  
4. Sci/Tech  

---

🤖 Model Applied  
**BERT (bert-base-uncased)**  
- Pretrained transformer model from Hugging Face  
- Fine-tuned for 4-class news topic classification  

---

⚙️ Steps Performed  
1. **Data Preprocessing**  
   - Tokenization with Hugging Face AutoTokenizer  
   - Truncation and padding (max length = 128 tokens)  

2. **Model Training**  
   - Fine-tuned bert-base-uncased using Hugging Face Trainer API  
   - 3 epochs, learning rate = 2e-5  

3. **Evaluation**  
   - Metrics: Accuracy and Macro F1-score  

4. **Deployment**  
   - Built interactive **Gradio app** for live predictions  

---

📈 Key Results (Example)  
| Metric     | Score   |  
|------------|---------|  
| Accuracy   | ~0.94   |  
| F1-macro   | ~0.94   |  

*(Scores may vary slightly depending on seed & hardware)*  

---

🛠️ Skills Demonstrated  
- NLP using Hugging Face Transformers  
- Transfer learning & fine-tuning BERT  
- Evaluation with accuracy & F1-score  
- Model deployment with Gradio  

---

🚀 Future Improvements  
- Try faster models like DistilBERT or ALBERT  
- Add multilingual news datasets  
- Deploy using Streamlit or FastAPI  
- Explore advanced optimization (e.g., longer training, larger batch sizes)  

---

📂 File Structure  
