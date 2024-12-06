# DL-Text-Summarization

# Text Summarization Model Comparison Report

## Introduction

This project implements and compares two state-of-the-art transformer-based models for text summarization: T5 (Text-to-Text Transfer Transformer) and BART (Bidirectional and Auto-Regressive Transformers). Both models were evaluated on their ability to generate concise and accurate summaries while maintaining the essential information from the original text.

## Implementation Details

The implementation included:
- Fine-tuning both T5 and BART models for summarization
- Creating a comparison framework using Gradio interface
- Implementing comprehensive evaluation metrics
- Developing an interactive demo for real-time testing

## Performance Analysis

### Quantitative Metrics

Based on the evaluation results, here are the key metrics for both models:

| Metric | Original | T5 | BART |
|--------|----------|-----|------|
| Word Count | 44 | 30 | 43 |
| Compression Rate | 0% | 31.8% | 2.3% |
| ROUGE-1 | - | 81.08% | 98.85% |
| ROUGE-2 | - | 80.56% | 98.82% |
| ROUGE-L | - | 81.08% | 98.85% |

### Model Characteristics

**T5 Model Performance**:
- Achieved significant compression (31.8%)
- Maintained good ROUGE scores (around 81%)
- Demonstrated effective information distillation
- Better suited for tasks requiring substantial summarization

**BART Model Performance**:
- Minimal compression (2.3%)
- Exceptional ROUGE scores (>98%)
- Nearly perfect preservation of original content
- Ideal for high-fidelity text preservation tasks

## Comparative Analysis

### Strengths and Trade-offs

1. **Compression Efficiency**:
   - T5 shows superior compression while maintaining content quality
   - BART prioritizes content preservation over length reduction

2. **Summary Quality**:
   - BART achieves near-perfect ROUGE scores
   - T5 balances between compression and content preservation

3. **Use Case Suitability**:
   - T5: Better for applications requiring shorter summaries
   - BART: Optimal for tasks requiring high-fidelity content preservation

## Conclusion

The evaluation reveals distinct characteristics of each model:
- T5 excels at generating concise summaries while maintaining good quality
- BART provides highly accurate summaries with minimal information loss
- Choice between models should depend on specific use case requirements regarding compression vs. accuracy trade-offs

The results demonstrate that both models have their unique strengths, making them suitable for different summarization scenarios depending on the specific requirements of the application.
