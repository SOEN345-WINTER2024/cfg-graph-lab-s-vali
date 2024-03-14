Sofia Valiante 40191897


## Android App
Method:
protected void applyCustomTheme() {
        binding.commentCoordinatorLayout.setBackgroundColor(mCustomThemeWrapper.getBackgroundColor());
        applyAppBarLayoutAndCollapsingToolbarLayoutAndToolbarTheme(binding.commentAppbarLayout, null, binding.commentToolbar);
        binding.commentParentTitleTextView.setTextColor(customThemeWrapper.getPostTitleColor());
        binding.commentDivider.setBackgroundColor(mCustomThemeWrapper.getDividerColor());
        binding.commentCommentEditText.setTextColor(mCustomThemeWrapper.getCommentColor());
        int secondaryTextColor = mCustomThemeWrapper.getSecondaryTextColor();
        binding.commentCommentEditText.setHintTextColor(secondaryTextColor);
        if (isReplying) {
            parentTextColor = mCustomThemeWrapper.getCommentColor();
        } else {
            parentTextColor = mCustomThemeWrapper.getPostContentColor();
        }
        parentSpoilerBackgroundColor = parentTextColor | 0xFF000000;
        binding.commentAccountNameTextView.setTextColor(mCustomThemeWrapper.getPrimaryTextColor());

        if (typeface != null) {
            binding.commentCommentEditText.setTypeface(typeface);
        }
        if (titleTypeface != null) {
            binding.commentParentTitleTextView.setTypeface(titleTypeface);
        }
    }

1) CFG

![code2flow_aotaKM](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-s-vali/assets/91510546/9701a6eb-4d00-46ef-b1f3-dcd5dcdfe3b9)

2) 
