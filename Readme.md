# OIDC gives temporary credentials

1. Storing Access keys is risky
2. Long lived credentials
3. Rotation head-ache
4. Keys can leak


Old:

GitHub → Stored AWS Keys → AWS

New:

GitHub → OIDC Token → AWS Temporary Access


Simple flow:

1️⃣ GitHub generates identity token
2️⃣ AWS verifies token
3️⃣ AWS gives temporary permissions
4️⃣ Workflow deploys securely

#WHy companies use this?
Large companies want to reduce the risk of leaked credentials.

That’s why OIDC is becoming standard in modern DevOps pipelines.



So DevOps today is not just automation…
it’s secure automation.