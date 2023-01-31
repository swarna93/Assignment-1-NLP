
def separate_words(Lines):
     cwords = []
     incwords = []
     crr_spell = ''
     icrr_spell = ''
     for line in Lines:
         if '$' in line:
              crr_spell = line.replace('$', '').replace('\n', '').lower()
         else:
              incrr_spell = line.lower().replace('\n', '')
              cwords.append(crr_spell)
              incwords.append(incrr_spell)
     return cwords, incwords

