# 3
import random

# 1から100の間の数字をランダムに1つ決定
correct_answer = random.randint(1, 100)
print("【数当てゲーム】1から100の数字を当ててみてね！")

# 当たるまで繰り返す
while True:
    # 画面から数字を入力（※スマホの環境によっては入力画面がポップアップします）
    user_guess = int(input("予想する数字を入力してください: "))
    
    if user_guess < correct_answer:
        print("もっと【大きい】数字だよ！ ⬆️")
    elif user_guess > correct_answer:
        print("もっと【小さい】数字だよ！ ⬇️")
    else:
        print("おめでとうございます！大正解です🎉")
        break  # ゲーム終了
