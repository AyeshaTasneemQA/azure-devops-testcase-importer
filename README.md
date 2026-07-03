I spent hours trying to import multi-step test cases into Azure DevOps Test Plans via CSV.

46 test cases turned into 130 broken duplicates. Steps missing. Expected results gone. Every format I tried — same result.

Turns out the built-in CSV importer doesn't correctly populate the Steps field on certain Azure DevOps configurations. It's a known limitation that almost nobody documents clearly.

So I built a Python script that bypasses the importer entirely and uses the REST API instead — creating each test case with all steps, actions, and expected results correctly structured. 46 test cases, all steps intact, linked to the right suite, done in seconds.

I've open sourced it for any QA engineer hitting the same wall 👇

🔗 GitHub: https://github.com/AyeshaTasneemQA/azure-devops-testcase-importer

Full breakdown of the problem, root cause, and how the script works in my latest article — link in comments.

If this saves you time, feel free to share it with your team 🙌

#AzureDevOps #QualityAssurance #SoftwareTesting #QAEngineer #TestAutomation #Python #DevOps #TestManagement #Agile #Pakistan
