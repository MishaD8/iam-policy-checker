# 🔑 IAM Policy Checker

## 📖 Description
This project provides a script that scans all IAM policies in your AWS account and detects **overly permissive policies** that could create security risks.

## 🎯 Project Goals
- Automatically download all existing IAM policies.
- Analyze policies for risky permissions (like Allow *:*).
- Generate a CSV report with security recommendations.

## ⚙️ Technologies Used
- AWS CLI
- Python (boto3, json)
- CSV (for the report)

## 📂 Files
| File | Description |
|---|---|
| policy_checker.py | Main analysis script |
| risk_patterns.json | List of risky permissions to check for |
| README.md | Project documentation |

## 🚀 How to Use
1. Make sure AWS CLI is configured.
2. Run the script:  
   `python policy_checker.py`
3. Review generated `iam_policy_report.csv`.

## 🔗 Useful Links
- [AWS IAM Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)
- [boto3 Documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)
