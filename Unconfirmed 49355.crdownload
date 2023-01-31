def ret_success(correct_words,incorrect_words,results):
	success = {}
	f=0
	k=0
	for i in range (len(results)):
		if (results[i][0][0] == correct_words[i]):
			success[incorrect_words[i]] = {'success_1':1, 'success_5':1, 'success_10':1}
		else:
			k=0

			for j in range(5):
				if (results[i][1][j] == correct_words[i]):
					success[incorrect_words[i]] = {'success_1':0, 'success_5':1, 'success_10':1}
					k=1
					break

			if(k==1):  
				continue
			f=0
			for j in range(10):
				f=f+1
				if (results[i][2][j] == correct_words[i]):
					success[incorrect_words[i]] = {'success_1':0, 'success_5':0, 'success_10':1}
					break
				if(f==10):
					success[incorrect_words[i]] = {'success_1':0, 'success_5':0, 'success_10':0}       
	return success
