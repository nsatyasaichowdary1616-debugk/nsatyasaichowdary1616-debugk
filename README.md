mkdir -p yourusername/.github/workflows yourusername/assets
cd yourusername

cat > README.md << 'EOF'
PASTE README.md CONTENT HERE
EOF

cat > .github/workflows/snake.yml << 'EOF'
PASTE snake.yml CONTENT HERE
EOF

cat > assets/orbit-banner.svg << 'EOF'
PASTE orbit-banner.svg CONTENT HERE
EOF

git init
git add .
git commit -m "Initial profile"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.git
git push -u origin main
