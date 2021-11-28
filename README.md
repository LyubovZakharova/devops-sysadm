# devops-sysadm

1.	Oracle VB: 
sudo apt update && sudo apt install virtualbox
2.	Vagrant(по их инструкции): 
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt install vagrant
3.СМ.ПАПКУ images	
4.	
mkdir VagrantVM
C:\VM's>cd vagrantvm
C:\VM's\VagrantVM>vagrant init bento/ubuntu-20.04
A `Vagrantfile` has been placed in this directory. You are now
ready to `vagrant up` your first virtual environment! Please read
the comments in the Vagrantfile as well as documentation on
`vagrantup.com` for more information on using Vagrant.
C:\VM's\VagrantVM>notepad vagrantfile
C:\VM's\VagrantVM>vagrant up
СМ.ПАПКУ images
#  выключить ВМ с сохранением ее состояния – vagrant suspend
#  выключить ВМ штатным образом- vagrant halt
5.	Оперативная память 1024МБ; 64,00 ГБ диском
СМ.ПАПКУ images
6.	Документация в VagrantFile предлагает прописать так:
config.vm.provider "virtualbox" do |v|
  v.memory = 1024   # требуемая оперативная память
  v.cpus = 2   # требуемое количество процессоров
end
7.	Выход из машины командой exit
СМ.ПАПКУ images
8.СМ.ПАПКУ images
9.СМ.ПАПКУ images
Ignoreboth – одна из возможностей определить правила сохранения команд в списке history. Это одно из значений, которое может входить в список, содержащихся в переменной HISTCONTROL. 
- если в списке указано ignorespace, то в истории не сохраняются строки, начинающиеся с пробела;
- если указано ignoredups, то в истории не сохраняются команды, повторяющиеся несколько раз подряд. 
ignoreboth - сокращение, которое объединяет в себе две предыдущие директивы.
# 117 строка у меня
RESERVED WORDS
       Reserved words are words that have a special meaning to the shell.  The following words are recognized as reserved when unquoted and either the first word of a simple command (see SHELL GRAMMAR  be?
       low) or the third word of a case or for command:
       ! case  coproc  do done elif else esac fi for function if in select then until while { } time [[ ]]
# 764 строка у меня
Brace Expansion
       Brace  expansion  is  a mechanism by which arbitrary strings may be generated.  This mechanism is similar to pathname expansion, but the filenames generated need not exist.  Patterns to be brace ex?
       panded take the form of an optional preamble, followed by either a series of comma-separated strings or a sequence expression between a pair of braces, followed by an optional postscript.  The  pre?
       amble is prefixed to each string contained within the braces, and the postscript is then appended to each resulting string, expanding left to right.
       Brace expansions may be nested.  The results of each expanded string are not sorted; left to right order is preserved.  For example, a{d,c,b}e expands into `ade ace abe'.
       A  sequence expression takes the form {x..y[..incr]}, where x and y are either integers or single characters, and incr, an optional increment, is an integer.
10.	 300000  -  создать невозможно, так как слишком большой список аргументов
СМ.ПАПКУ images
11.	 Конструкция оценивает утверждение "/tmp - это директория" на предмет истины или лжи
СМ.ПАПКУ images
12.СМ.ПАПКУ images
13.
at позволяет задать время выполнения команды или скрипта (задача выполняется один раз в установленное время).
atq позволяет просмотреть список задач, поставленных пользователем.
batch позволяет назначить выполнение задачи на момент, когда загруженность минимальна. По умолчанию в качестве порога используется значение load average < 1.5
(синтаксически используется так же, как at)
