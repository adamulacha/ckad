sudo -i
# autocompletion
# you will get it from here: https://kubernetes.io/docs/reference/kubectl/cheatsheet/#kubectl-autocomplete
source <(kubectl completion bash)
echo "source <(kubectl completion bash)" >> ~/.bashrc
alias k=kubectl
complete -F __start_kubectl k

# env variables
export do="--dry-run=client -oyaml"
export now="--grace-period=0 --force"

# aliases
alias current-ns="k config view --minify | grep namespace"
alias change-ns="k config set-context --current --namespace" # that was really useful! I didn't use -n switch.

# vim setup
vim .vimrc
set nu ruler expandtab ts=2 sw=2
source .vimrc
