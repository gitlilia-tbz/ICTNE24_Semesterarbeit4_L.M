cat > secrets/README.md << 'EOF'
# Secrets Directory

⚠️ **WICHTIG:** Dateien in diesem Verzeichnis werden NICHT in Git committed!

## Secrets erstellen
```bash
# Database Secret
kubectl create secret generic postgres-credentials \
  --from-literal=username=postgres \
  --from-literal=password=sicheres-passwort \
  -n trackmygym

# API Keys (falls benötigt)
kubectl create secret generic api-keys \
  --from-literal=openweather-api-key=dein-api-key \
  -n trackmygym
```

## Secrets anzeigen
```bash
# Liste aller Secrets
kubectl get secrets -n trackmygym

# Secret Details
kubectl get secret postgres-credentials -o yaml -n trackmygym
```
EOF
